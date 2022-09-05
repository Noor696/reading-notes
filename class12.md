## CRUD 
### Create, read, update and delete

### Reading
[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

**1 - In your own words, describe what each group of status code represents:**

 - 100's = Informational codes used to relay information between client and server during a request. 
 - 200's = success codes. These indicate that the request issued was successfully fulfilled.
 - 300's = redirect codes. These codes are used to tell the browser or server that some other action needs to take place to complete the previous request.
 - 400's = client errors. These indicates an error on the requesters behalf.
 - 500's = server errors. These indicates an error on the servers behalf.


**2- What is a status code 202?**
Accepted response status code indicates that the request has been accepted for processing, but the processing has not been completed.

**3- What is a status code 308?**
308 Permanent Redirect redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers.

**4- What code would you use if an update didn't return data to a client?**
204

**5- What code would you use if a resource used to exist but no longer does?**
409

**6- What is the 'Forbidden' status code?**
4.3

### Videos
[Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

**1- Why do we need to pull our MongoDB database string out of our server and put it into our .env?**
It is hidden and no one can use it or change it

**2- What is middleware?**
Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.(1)

**3- What does app.use(express.json()) do?**
The app.use() function adds a new middleware to the app. Essentially, whenever a request hits your backend, Express will execute the functions you passed to app.use(),,It parses incoming JSON requests and puts the parsed data in req.

**4- What does the /:id mean in a route?**
Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

**5- What is the difference between PUT and PATCH?**

| PUT  | PATCH   |
| ------------- | ------------- |
| PUT is a method of modifying resource where the client sends data that updates the entire resource . | PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data. |
| It has High Bandwidth  | Since Only data that need to be modified if send in the request body as a payload , It has Low Bandwidth  |
| In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced | With PATCH, however, the enclosed entity contains a set of instructions describing how a resource currently residing on the origin server should be modified to produce a new version. |
| HTTP PUT is said to be idempotent, So if you send retry a request multiple times, that should be equivalent to a single request modification | HTTP PATCH is basically said to be non-idempotent. So if you retry the request N times, you will end up having N resources with N different URIs created on the server. |

(2)

**6- How do you make a default value in a schema?**
Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.


**7- What does a 500 error status code mean?**
It means that the server encountered an unexpected condition that prevented it from fulfilling the request

**8- What is the difference between a status 200 and a status 201?**
The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created.


## References
_______
(1)
[topics/middleware](https://www.redhat.com/en/topics/middleware/what-is-middleware)

(2)
[difference-between-put-and-patch-request](https://www.geeksforgeeks.org/difference-between-put-and-patch-request/)

