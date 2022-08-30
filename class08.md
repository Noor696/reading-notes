## APIs

(API Design Best Practices)[https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design]

**What does REST stand for?**
Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia.

**REST APIs are designed around a _resources_.**

**What is an identifier of a resource? Give an example.**
is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

https://adventure-works.com/orders/1

**What are the most common HTTP verbs?**
The most common operations are GET, POST, PUT, PATCH, and DELETE.

**What should the URIs be based on?**
resources , The only place where information is stored is in the resources themselves

**Give an example of a good URI.**
https://www.adventure-works.com/

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**
"chatty" web APIs that expose a large number of small resources. _bad_


**What status code does a successful GET request return?**
A successful GET method typically returns HTTP status code 200 (OK).

**What status code does an unsuccessful GET request return?**
If the resource cannot be found, the method should return 404 (Not Found).

**What status code does a successful POST request return?**
it returns HTTP status code 201 (Created)

**What status code does a successful DELETE request return?**
If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content).