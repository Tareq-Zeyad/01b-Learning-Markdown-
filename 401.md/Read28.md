# Django Forms
![forms](https://i.stack.imgur.com/5x3Ck.png)

# What are Django Forms ?

- A Form class which is used to create HTML forms. It describes a form and how it works and appears. It is similar to the ModelForm class that creates a form by using the Model, but it does not require the Model.

# What Django Forms used for ?

- Forms are basically used for taking input from the user in some manner and using that information for logical operations on databases. For example, Registering a user by taking input as his name, email, password, etc. Django maps the fields defined in Django forms into HTML input fields

# How does Django handle input process ?


Explained in this diagram:

![diagram](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms/form_handling_-_standard.png)

1. Display the default form the first time it is requested by the user.
* The form may contain blank fields (e.g. if you're creating a new record), or it may be pre-populated with initial values (e.g. if you are changing a record, or have useful default initial values).
* The form is referred to as unbound at this point, because it isn't associated with any user-entered data (though it may have initial values).
2. Receive data from a submit request and bind it to the form.
Binding data to the form means that the user-entered data and any errors are available when we need to redisplay the form.
Clean and validate the data.
* Cleaning the data performs sanitization of the input (e.g. removing invalid characters that might be used to send malicious content to the server) and converts them into consistent Python types.
* Validation checks that the values are appropriate for the field (e.g. are in the right date range, aren't too short or too long, etc.)
4. If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.
5. If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)
6. Once all actions are complete, redirect the user to another page.
