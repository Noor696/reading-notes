## Django CRUD and Forms

### Django Forms 
[Django Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)


* HTML Form can be used to collect information from users for submission to a server. 

* Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data (text boxes, checkboxes, radio buttons, date pickers, ...).

* Forms are a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

* Django Forms providing a framework that lets you define forms and their fields programmatically, and then use these objects to both generate the form HTML code and handle much of the validation and user interaction.

* some important deffenition in **html form**:
 
    - **action**: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.

    - **method**: The HTTP method used to send the data: post or get:

       - The **POST method** should always be used if the data is going to result in a change to the server's database, because it can be made more resistant to cross-site forgery request attacks.

       - The **GET method** should only be used for forms that don't change user data (for example, a search form). It is recommended for when you want to be able to bookmark or share the URL.

### **Django form handling process:**

* gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page

* the main things that Django's form handling does are:
  
  - Display the default form the first time it is requested by the user.

  - Receive data from a submit request and bind it to the form (the user-entered data and any errors are available when we need to redisplay the form.)

  - Clean and validate the data

  - If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.

  - If all data is valid, perform required actions (such as save the data, send an email, return the result of a search, upload a file, and so on).

  - Once all actions are complete, redirect the user to another page.

### Form fields

The arguments that are common to most fields:

* required
* label
* label_suffix
* initial
* widget
* help_text
* error_messages
* validators
* localize
* disabled

