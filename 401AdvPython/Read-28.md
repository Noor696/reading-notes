## Read 28 : Authentication & Production Server

[JSON Web Tokens](https://jwt.io/introduction/)

* **JSON Web Token (JWT)** is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

* JWTs can be **signed** using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

* JSON Web Tokens are useful in some scenarios :

  - Authorization
  - Information Exchange

* JSON Web Token structure : JSON Web Tokens consist of three parts separated by dots (.), which are:

 - **Header** : header typically consists of two parts 
     - type of the token (ex: "typ": "JWT")
     - signing algorithm being used (ex :"alg": "HS256").

 - **Payload** : contains the claims. Claims are statements about an entity (typically, the user) and additional data:
     - Registered claims: These are a set of predefined claims which are not mandatory but recommended, to provide a set of useful, interoperable claims.

     - Public claims: These can be defined at will by those using JWTs. 

     - Private claims: These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

 - **Signature** : To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

 ------------------------------


[DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

* The JWT is just an authorization token that should be included in all requests.

* The JWT is acquired by exchanging an username + password for an access token and an refresh token.

  - The **access token** is usually short-lived

  - The **refresh token** lives a little bit longer

* three distinctive parts that compose a JWT:

> header.payload.signature

* using the **djangorestframework_simplejwt** library, recommended by the DRF developers.

> pip install djangorestframework_simplejwt

* settings.py: 
> REST_FRAMEWORK = {
    'DEFAULT_AUTHENTICATION_CLASSES': [
        'rest_framework_simplejwt.authentication.JWTAuthentication',
    ],
}

* urls.py:
> from rest_framework_simplejwt import views as jwt_views
urlpatterns = [
    # Your URLs...
    path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
    path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
]

-------------------------------------

[Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)

* So the server started with runserver is not guaranteed to be performant (it’s very slow), and it hasn’t been built with security concerns in mind.

* You want to only use tech in production, which is reliable, well tested and has been around for a while.

* Django app does not actually run as you would think a server would - waiting for requests and reacting to them. Your project provides a uwsgi.py file, which contains a function to be called by the application server. This function gets a Python object representing the incoming request.