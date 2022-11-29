## Readings: Django Models

**Using models**
[Using models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)

* Django web applications access and manage data through Python objects referred to as models.

* Models define the structure of stored data.

* The definition of the model is independent of the underlying database.

**Designing the LocalLibrary models:**

* When designing your models, it makes sense to have separate models for every "object" (a group of related information)

* might also want to use models to represent selection-list options (e.g. like a drop down list of choices)

* rather than hard coding the choices into the website itself.

* Once we've decided on our models and field, we need to think about the relationships.

* Django allows you to define relationships that are 
  - one to one (OneToOneField)
  - one to many (ForeignKey)  
  - many to many (ManyToManyField)

**Model primer:**

* Model definition: Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

* Fields: A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

* COMMON FIELD ARGUMENTS: 

  - help_text: Provides a text label for HTML forms 
  - verbose_name: A human-readable name for the field used in field labels. 
  - default: The default value for the field. This can be a value or a callable object.
  - null: If True, Django will store blank values as NULL in the database for fields where this is appropriate. The default is False.
  - blank: If True, the field is allowed to be blank in your forms. The default is False
  - choices: A group of choices for this field. 
  - primary_key: If True, sets the current field as the primary key for the model . If no field is specified as the primary key, Django will automatically add a field for this purpose.

**Django admin site**
[Django admin site](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

* The Django admin application can use your models to automatically build a site area that you can use to create, view, update, and delete records. 

* The admin application can also be useful for managing data in production, depending on the type of website.

* all you must do to add your models to the admin application is to register them.

* Registering models:
  
  - open admin.py
  - Register the models by copying (from .models import Author, Genre, Book, BookInstance) into the bottom of the file.
  - calls (admin.site.register) to register each of them.