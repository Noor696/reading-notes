## REST

[How I explained REST to my brother](https://gist.github.com/brookr/5977550)

**1. Who is Roy Fielding?**
Roy Fielding is programmer helped write the first web servers, that sent documents across the interne, and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

**2. Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?**
URLs tell the browser that there's a concept, somewhere. A browser can then go ask for a specific representation of the concept. Specifically, the browser asks for the web page representation of the concept.
Actually, representations is one of these things that doesn't get used a lot. In many cases, a resource has only a single representation.

**3. What is the HTTP protocol that Fielding and his friends created?**
Hypertext Transfer Protocol (HTTP), is the foundation of data communication for the World Wide Web, where hypertext documents include hyperlinks to other resources that the user can easily access,

**4. What does a GET do?**
Retrieve a representation of a resource in a specified  representation (Internet media type).


**5. What does a POST do?**
Use the data in the request body to modify a resource. The  URI identifies a resource that will handle the enclosed data.


**6. What does PUT do?**
The body of the request creates or sets the current state of a  resource identified by the URI.


**7. What does PATCH do?**
it applies partial modifications.