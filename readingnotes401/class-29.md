# Django Custom User Models

## Setting Up a User

To begin, you need to create the user before you run migrations. Two types of users. AbstractUser or AbstractBaseUser in which case AbstractBaseUser means that we will need to implement more work.

These are the steps needed to compete to create the base user:

* update django_project/settings.py
* create a new CustomUser model
* create new UserCreation and UserChangeForm
* update the admin

An example of what this code will look like is this:

``` python
# accounts/models.py
from django.contrib.auth.models import AbstractUser
from django.db import models

class CustomUser(AbstractUser):
    pass
    # add additional fields in here

    def __str__(self):
        return self.username
```

We need to update the forms.py after this to implement it with the user. This is done in an example below:

``` python

# accounts/forms.py
from django import forms
from django.contrib.auth.forms import UserCreationForm, UserChangeForm

from .models import CustomUser

class CustomUserCreationForm(UserCreationForm):

    class Meta:
        model = CustomUser
        fields = ("username", "email")

class CustomUserChangeForm(UserChangeForm):

    class Meta:
        model = CustomUser
        fields = ("username", "email")
```

Finally we update our admin. Here is the sample code for that:

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
    list_display = ["email", "username",]

admin.site.register(CustomUser, CustomUserAdmin)
```

## Things I want to know more about

### Resources

[Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

### Links

- >[Advanced Software Development](README.md)
