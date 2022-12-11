## Readings: Django REST Framework & Docker

[Beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

[Django for APIs - Library Website](https://djangoforapis.com/library-website-and-api/)

[Videos - Beginner's Guide to Django REST Framework]()

* With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally. And Docker can be shared among team members so everyone is working on the same setup.

* Docker is really just Linux containers which are a type of virtualization.

* To install Docker we need to download the desktop app on our computer and create a free account. --> Once Docker is done installing we can confirm the correct version is running. It should be at least version 19.

* Docker Compose is an additional tool that is automatically included with Mac and Windows downloads of Docker, on Linux, you will need to add it manually by running the command 'sudo pip install docker-compose' after your Docker installation is complete.

* To confirm Docker installed correctly we can run our first command 'docker run hello-world'. 

-----------------

* Django REST Framework works alongside the Django web framework to create web APIs.

*  Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

* 
> cd onedrive\desktop\code
> mkdir library
> cd library
> python -m venv .venv
> .venv\Scripts\Activate.ps1
(.venv) > python -m pip install django~=4.0.0

* create a new project with the startproject command called django_project. Don’t forget to include the period . at the end which installs the code in our current directory. If you do not include the period, Django will create an additional directory by default.

(.venv) > django-admin startproject django_project .

* then complete all steps to create django app.