## Authentication

**Reading**

[What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

**1- What is OAuth?**
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

**2- Give an example of what using OAuth would look like.**
you're using an app on Facebook, and it asks you to share your profile and pictures. Facebook is, in this case, the service provider: it has your login data and your pictures.

**3- How does OAuth work? What are the steps that it takes to authenticate the user?**
- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- The first site gives this token and secret to the initiating user’s client software.
- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
- The user approves (or their software silently approves) a particular transaction type at the first website.
- The user is given an approved access token (notice it’s no longer a request token).
- The user gives the approved access token to the first website.
- The first website gives the access token to the second website as proof of authentication on behalf of the user.
- The second website lets the first website access their site on behalf of the user.
- The user sees a successfully completed transaction occurring.
- OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

**4- What is OpenID?**
OpenID began life in 2005 as a means for logging into the then-popular LiveJournal blogging site but quickly spread to other sites.


[Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

**What is the difference between authorization and authentication?**
- Authorization is the security process that determines a user or service's level of access. In technology, we use authorization to give users or services permission to access some data or perform a particular action. 
- Authentication (AuthN) is a process that verifies that someone or something is who they say they are. Technology systems typically use some form of authentication to secure access to an application or its data.

_authentication and authorization may sound alike, but each plays a different role in securing systems and data. Unfortunately, people often use both terms interchangeably as they both refer to system access. However, they are distinct processes. Simply put, one verifies the identity of a user or service before granting them access, while the other determines what they can do once they have access._


**What is Authorization Code Flow?**
Authorization code flow is used to obtain an access token to authorize API requests. Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API.


**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**
The Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users. 


**What is Implicit Flow with Form Post?**
Form Post flow uses OIDC to implement web sign-in

**What is Client Credentials Flow?**
In the client credentials flow, permissions are granted directly to the application itself by an administrator.


**What is Device Authorization Flow?**
With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text.

**What is Resource Owner Password Flow?**
The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. This flow has significantly different security properties than the other OAuth flows.


## References

[authentication-vs-authorization](https://www.onelogin.com/learn/authentication-vs-authorization)