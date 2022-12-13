## Permissions & Postgresql

* Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.

* permissions determine whether a request should be granted or denied access, Permissions are used to grant or deny access for different classes of users to different parts of the API.

* Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

*  **IsAuthenticated ** class in REST framework:
The simplest style of permission to allow access to any authenticated user, and deny access to any unauthenticated user.

* **IsAuthenticatedOrReadOnly** class in REST framework:
A slightly less strict style of permission to allow full access to authenticated users, but allow read-only access to unauthenticated users. 

* Permissions in REST framework --> list of permission classes.

* **How permissions are determined:**

  - Before running the main body of the view -->
  - checked each permission in the list -->
  - if permission check fails, an **exceptions.PermissionDenied** or **exceptions.NotAuthenticated** exception will be raised. --> the main body of the view will not run. -->
  - response will be returned **"403 Forbidden"** or a **"401 Unauthorized"**