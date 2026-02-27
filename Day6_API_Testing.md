**API is an Application Programming Interface** is a set of rules or protocols that enable software applications to communicate with each other to exchange data, features, and functionality.

Example:

1. Frontend sends a request
2. Backend process
3. Database returns data
4. API sends response

Unlike UI testing, API testing focuses on backend logic.



API communicates in terms of requests and responses between a client and server. The application submitting request is the client, and the server provides the response. API works as a bridge between the client and the server.

&nbsp;	Request		Response

Client --------> API <----------- Server



**Components of an API**

1. **Endpoints-** URL that provides access to specific features/functionality.
2. **Methods/HTTP verbs-** Actions that can be performed(Eg: GET, POST, PUT, DELETE)
3. **Request(method, headers, body, auth)-** Data sent by the client to the server
4. **Response(status code, body, schema)-** Data sent back by the server to the client
5. **Header-** Metadata about the request or response(Eg: Authentication token, content type)
6. **Payload/Body-** Data being sent with request(typically in JSON or in XML)



status codes returned by APIs

* 200 OK: The request was successful.
* 201 Created: A new resource was successfully created.
* 203 Non-Authoritative Information 
* 204 No Content: The request was successful, but there is no content to return.
* 400 Bad Request: The request was invalid or cannot be processed.
* 401 Unauthorized: Authentication is required and has failed or not been provided.
* 403 Forbidden: The server understands the request but refuses to authorize it.
* 404 Not Found: The requested resource could not be found.
* 409: Conflict
* 500 Internal Server Error: An error occurred on the server side.
* 501: Not Implemented
* 502: Bad Gateway
* 503: Service Unavailable
* 504: Gateway Timeout
* 599: Network Timeout 



**HTTP methods** 

**GET-** Retrieve data from the server 

Example: **GET https://jsonplaceholder.typicode.com/posts/1**

Check:

Status code → **200**

Response body fields

Response time

Content-Type header



**POST-** Create a new resource or submit data to the server

Example: **POST https://jsonplaceholder.typicode.com/posts**

Body:

{

&nbsp; "title": "API Testing",

&nbsp; "body": "Learning Postman",

&nbsp; "userId": 1

}

Check:

Status code → **201 (Created)**

Response contains new ID

Validate request payload matches response



**PUT-** Update existing resource on the server

Example: **PUT https://jsonplaceholder.typicode.com/posts/1**

Body:

{

&nbsp; "id": 1,

&nbsp; "title": "Updated Title",

&nbsp; "body": "Updated body",

&nbsp; "userId": 1

}

Check:

Status code → **200**

Entire record replaced



**PATCH-** Apply partial modification to a resource 

Example: **PATCH https://jsonplaceholder.typicode.com/posts/1**

Body:

{

&nbsp; "title": "Partially Updated"

}

Only updates one field.



**DELETE-** Remove a resource from the server

Example: **DELETE https://jsonplaceholder.typicode.com/posts/1**

Check:

Status code → **200 or 204**



**REST (Representational State Transfer):**

* Uses standard HTTP methods (GET, POST, PUT, DELETE).
* Stateless, meaning each request from a client to a server must contain all the information needed to understand and process the request.
* Typically uses JSON or XML for data interchange.
* It is easier to implement and more scalable for web services.
* 
**SOAP (Simple Object Access Protocol):**

* A protocol-based approach that relies on XML for message format.
* Includes built-in error handling and supports more complex operations.
* Uses stricter standards and can work over several protocols (HTTP, SMTP, TCP).
* Generally more secure with built-in security features.



