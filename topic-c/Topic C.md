# Topic C - Client Server Interaction

## Objectives

-   Understanding Serialisation and Deserialisation
-   Api's url format conventions
-   Method Idempotence
-   Validation of API
-   Authenticating without Password
-   Authentication & Authorization
-   Rate-limiting / Throttling
-   OAuth2 & Owin
-   HTTP Statelessness
-   REST Api Security Principles (Read yourself)
-   JWT Token demo
-   Web Identity Federation
-   AJAX

## Understanding Serialisation and Deserialisation

> Serialization is the process of converting an object into a stream of bytes to store the object or transmit it to memory, a database, or a file. Its main purpose is to save the state of an object in order to be able to recreate it when needed. The reverse process is called deserialization. - [Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/serialization/)

-   JSON context
    -   Serialisation: From JSON to string
    -   Deserialisation: From string to JSON

## API's URL Format Conventions

-   `/api/[version]/[controller]/{id}`
    -   [version] - to avoid conflicts for older api versions
    -   [controller] - in plural form
    -   {id} - the id of the resource you wish to get (optional)

#### GET

-   `/api/v1/Schools`
    -   Returns all schools
-   `/api/v1/Schools/SingaporePolytechnic`
    -   Returns the specified school

#### POST

-   `/api/v1/Schools`
    -   Creates a school based on the payload in the request

#### PUT

-   `/api/v1/Schools/SingaporePolytechnic`
    -   Updates the specified resource with the payload in the request

#### DELETE

-   `/api/v1/Schools/SingaporePolytechnic`
    -   Deletes the specified resource from the server

### Resource Relations

#### GET

-   `/api/v1/Schools/SingaporePolytechnic/Students`
    -   Returns a all student in the specified school
-   `/api/v1/Schools/SingaporePolytechnic/Students/P1742554`
    -   Returns the specified student in the specified school
-   `/api/v1/Schools/SingaporePolytechnic/Staffs`
    -   Returns a all student in the specified school
-   `/api/v1/Schools/SingaporePolytechnic/Staffs/S57899`
    -   Returns the specified staff in the specified school

### Filtering

#### GET

-   `/api/v1/Schools?limit=3`
    -   return the first 3 schools
-   `/api/v1/Schools?offset=20`
    -   Skip the first 20 schools and return the rest
-   `/api/v1/Schools?offset=20&limit=10`
    -   Skip the first 20 schools and return the next 10 schools
-   `/api/v1/Schools?offset=55&limit=100`
    -   Skip the first 55 schools and return the next 100 schools

<sub><sup>Order by name / education level?</sup></sub>

## Method Idempotence

> A request method is considered "idempotent" if the intended effect on the server of multiple identical requests with that method is the same as the effect for a single such request. Of the request methods defined by this specification, PUT, DELETE, and safe request methods are idempotent. - [RFC7231](https://tools.ietf.org/html/rfc7231#section-4.2.2)

| Method  | Idempotent |
| ------- | ---------- |
| GET     | yes        |
| POST    | no         |
| PUT     | yes        |
| DELETE  | yes        |
| CONNECT | no         |
| HEAD    | yes        |
| OPTIONS | yes        |
| TRACE   | yes        |

## Validation of API

-   Built in ASP.NET validation
    -   ModelState
    -   Attributes

## Restful Security Best Practice

-   Validation - Validate all inputs on the server. Protect your server against SQL or NoSQL injection attacks.
-   Session based authentication - Use session based authentication to authenticate a user whenever a request is made to a Web Service method.
-   No sensitive data in URL - Never use username, password or session token in URL , these values should be passed to Web Service via POST method.
-   Restriction on Method execution - Allow restricted use of methods like GET, POST, DELETE. GET method should not be able to delete data.
-   Validate Malformed XML/JSON - Check for well formed input passed to a web service method.
-   Throw generic Error Messages - A web service method should use HTTP error messages like 403 to show access forbidden etc.

## Authenticating without Password

Authentication without password happens when a 3rd party application wishes to access a user's information on another application/server

### Ways to authenticate without password

-   OAuth
-   OpenId
-   SAML
-   FIDO

## Authentication and Authorization

Example: Blackboard

-   Attributes
    -   Authorize
        -   Users
        -   Roles
    -   AllowAnonymous

## Rate-limiting / Throttling

To mitigate abuse on the Api by limiting the number of reqests per seconds the user or application is allowed to make.

Example: [Google Directions Api](https://developers.google.com/maps/documentation/directions/usage-and-billing#other-usage-limits)

## HTTP Statelessness

## REST Api Security Principles (Read yourself)

[https://restfulapi.net/security-essentials/](https://restfulapi.net/security-essentials/)

## JWT Token demo

DEMO with pluralsight

## Amazon Web Identity Federation

![Web Identity Federation Diagram](https://blog.h4.nz/media/DelegationFederation/Standard%20Web%20Identity%20Federation.jpg)

## AJAX

Asynchronous Javascript And XML

Done via [XMLHttpRequest](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Using_XMLHttpRequest)

DEMO with jQuery and http://dummy.restapiexample.com

### Stripe Case Study

[![Stripe](https://img.youtube.com/vi/BQg267TuJ0M/0.jpg)](https://www.youtube.com/watch?v=BQg267TuJ0M)
