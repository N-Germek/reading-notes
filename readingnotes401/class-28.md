# Django Forms and CRUD

## Django forms, What are they?

Django forms are ways in which data can be gathered from the user in a group of input fields or widgets. It  can be displayed in a website or the information can be used to talk to the server. Forms allow us to send data to the server in POST requests which protects from cross site forgery requests.

## How do you write them?

Django forms are almost write themselves. By defining fields and their fields programatically, Django forms are built with the framework needed to create the site. Django will generate the HTML and handle the validation of the user action. The GET method should only be used for forms with  information that doesn’t change. The POST method is for information that will change.

## Django form Handling

Similar to others Django handling, the form handling of Django is for the server to get a request, fulfill the request and return an output of a rendered page. The steps in more detail are that Django will display the default form. Second, it will receive  the user input and populate the form. Third, it will clean and validate the data. Fourth, it will return the form with the data that was correct and error messages for the information that wasn’t. Once data is validated, the fifth step is to perform any actions programmed in. Finally, it will redirect to another page once all actions have been completed.

## Declaring a Form and Form Fields

This is similar to declaring a model in Django. Primary arguments included in the calling method include:

- Required: this field is required to have information otherwise it will throw an error. Fields cannon be left blank or be given a none value.

- Label: which is not specific and Django will create the field for you if nothing is specified. Django will create is based on the field and will capitalize the initial letter and replace underscores with spaces.

- Label_suffix: by default a colon is displayed unless specified.

- Initial: initial value when field is displayed.

- Widget: display widget that is to be used.

- Help_text: text information that can assist in completing the field.

- Error_message:  message displayed for errors and to explain what happened.

- Validators: functions that will be called to validate the field.

- Localized: localization. Of form data input.

- Disabled: this field is displayed but edits to it cannot be made.

## Validate a form

The `clean_<fieldname>()` method is the easiest way to validate the data. The two steps in the validating process is to declare `self.cleaned_data[<'field_data'>]` then return `self.cleaned_data[<'field_data'>]`.  Even if no changes are made to the data or form, this will return a validated set of information that is essentially cleaned.

## URL Configuration

Add in the configuration of the URL before updating your views so it can redirect you to the completed information after the actions have been completed.

## View

Similar to models, the views are needed to render the default data, process the data, or render the completed data with or without errors. When testing agains the POST request type in some forms, you would run `if request.method == 'POST'`. When testing the GET request, you would run an `else` condition.

## Templates

As we learned about templates earlier, this will be the time that any data that has been processed will be implemented in the template for a fully rendered site..

## ModelForm

This is the helper class when you are not looking to build an entire form page, but instead you are looking to insert a single form into a page of other content. This will already map to the correct locations because the builtins are equiped with assumptions of basic form data.

## CRUD

The `CreateView`, `UpdateView` and `DeleteView` are all builtin methogs in Django to accomplish CRUD. Create and Update both use the same template, where as Delete provides a separate template that is scrubbed or routs to anther page without the template integrated at all.

## Things I want to know more about

I would like to play with and learn more about the different types of field information in Django forms to see their limitations and identify when logic would be needed to override a builtin behavior and combine it with another field. For example, lerning what is the logic needed to create a form with a `BooleanField` combined with a `ChoiceField`.

### Resources

[Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

### Links

- >[Advanced Software Development](README.md)
