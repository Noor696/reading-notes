## Django Custom User


[Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)


[DjangoX](https://github.com/wsvincent/djangox)

* the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

* There are two modern ways to create a custom user model in Django: **AbstractUser and AbstractBaseUser.** In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much more work.

* So we'll use AbstractUser.



Creating our **initial custom user model** requires four steps:

* update django_project/settings.py
* create a new CustomUser model
* create new UserCreation and UserChangeForm
* update the admin

*  DjangoX, which is an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.

* DjangoX can be installed via Pip, Pipenv, or Docker. 

* To use Docker with PostgreSQL as the database update the DATABASES section of django_project/settings.py 