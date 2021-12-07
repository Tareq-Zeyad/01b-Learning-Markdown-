# **Django Custom User.**
![custom](https://testdriven.io/static/images/blog/django/django-custom-user-model/admin-site.png)
### What are Django Custom Users ?

- A built-in User model for authentication purposes such as logging in and out.

### What are the steps required for creating a Custom User Model ?

* update config/settings.py
* create a new CustomUser model
* create new UserCreation and UserChangeForm
* update the admin

1. 

In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call our custom user model CustomUser.

Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.

```python
# config/settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'accounts', # new
]
...
AUTH_USER_MODEL = 'accounts.CustomUser' # new
```
2. now update accounts/models.py with a new User model which we'll call CustomUser.

```python
# accounts/models.py
from django.contrib.auth.models import AbstractUser
from django.db import models

class CustomUser(AbstractUser):
    pass
    # add additional fields in here

    def __str__(self):
        return self.username
```
3. We need new versions of two form methods that receive heavy use working with users. Stop the local server with Control+c and create a new file in the accounts app called forms.py.

(accounts) $ touch accounts/forms.py
We'll update it with the following code to largely subclass the existing forms.

```python
# accounts/forms.py
from django import forms
from django.contrib.auth.forms import UserCreationForm, UserChangeForm
from .models import CustomUser

class CustomUserCreationForm(UserCreationForm):

    class Meta:
        model = CustomUser
        fields = ('username', 'email')

class CustomUserChangeForm(UserChangeForm):

    class Meta:
        model = CustomUser
        fields = ('username', 'email')
```
4. Finally we update admin.py since the Admin is highly coupled to the default User model.

```python
# accounts/admin.py
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin

from .forms import CustomUserCreationForm, CustomUserChangeForm
from .models import CustomUser

class CustomUserAdmin(UserAdmin):
    add_form = CustomUserCreationForm
    form = CustomUserChangeForm
    model = CustomUser
    list_display = ['email', 'username',]

admin.site.register(CustomUser, CustomUserAdmin)
```
And we're done! We can now run makemigrations and migrate for the first time to create a new database that uses the custom user model.

```bash
(accounts) $ python manage.py makemigrations accounts
(accounts) $ python manage.py migrate
```