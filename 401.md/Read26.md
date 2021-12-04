# **Intro to Django.**
## *Getting started with Django.*
### Django is a python web framework that allows to create web sites both on the client side and deploy it on the server side.Django takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It is free and open source, has a thriving and active community, great documentation, and many options for free and paid-for support.
![django](https://www.thecrazyprogrammer.com/wp-content/uploads/2018/08/Introduction-to-Django-1024x576.png)

<br>

## **Why Django ?**
### Because Django helps developers by speeding up the development process. It includes its own Object Relation Mapping (ORM) layer for handling database access, sessions, routing, and multi-language support. It also takes care of security while handling requests. It includes an admin panel (called django-admin) for managing models data by default.
<br>

## **Is Django Open Source & Who Maintains it ?**
### Django’s code is open source and available to all. Django’s organization is managed by a non-profit, the DSF, with a miniscule budget. And Django code is lead by a core team of volunteers, two paid Django Fellows, and a larger group of contributors.
<br>

## **Examples to use Django with Python**
### Forms:
- ### Django provides a powerful form library that handles rendering forms as HTML, validating user-submitted data, and converting that data to native Python types. Django also provides a way to generate forms from your existing models and use those forms to create and update data.
```
from django import forms

class BandContactForm(forms.Form):
    subject = forms.CharField(max_length=100)
    message = forms.CharField()
    sender = forms.EmailField()
    cc_myself = forms.BooleanField(required=False)
```
### Authentication: 
- ### Django comes with a full-featured and secure authentication system. It handles user accounts, groups, permissions and cookie-based user sessions. This lets you easily build sites that allow users to create accounts and safely log in/out.
```
from django.contrib.auth.decorators import login_required
from django.shortcuts import render

@login_required
def my_protected_view(request):
    """A view that can only be accessed by logged-in users"""
    return render(request, 'protected.html', {'current_user': request.user})
```
### Security:
### Django provides multiple protections against:
- ### Clickjacking
- ### Cross-site scripting
- ### Cross Site Request Forgery (CSRF)
- ### SQL injection
- ### Remote code execution
