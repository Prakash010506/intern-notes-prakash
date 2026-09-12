## 1. What is the HTTP protocol?

HTTP (Hypertext Transfer Protocol) is a protocol used for communication between a client and a server on the web. A client sends an HTTP request, and the server processes it and returns an HTTP response.

Example
A browser requests a webpage from a web server, and the server sends the webpage back as a response.

---

## 2. What is a web application?

A web application is a software application that runs on a web server and can be accessed by users through a web browser.

Example
Gmail, YouTube, and online banking websites are examples of web applications.

---

## 3. What is a web server?

A web server is a system that receives requests from clients and sends web content or responses back to them.

Example
When a browser requests a webpage, the web server receives the request and returns the required content.

---

## 4. What is the HTTPS protocol, and why is it considered secure?

HTTPS (Hypertext Transfer Protocol Secure) is the secure version of HTTP. It uses TLS to encrypt communication between a client and a server.

Example
When we enter a password on a website using HTTPS, the data is protected while travelling between the browser and server.

---

## 5. What is authentication, and what is authorization?

Authentication is the process of verifying the identity of a user.

Authorization is the process of deciding what an authenticated user is allowed to access or perform.

Example
Logging into an account with a username and password is authentication. Accessing an admin page based on your permissions is authorization.

---

6. How does social login work?

Social login allows users to sign in to an application using an account from an identity provider such as Google.

### Example
When a user selects "Sign in with Google", the user is redirected to Google for authentication. After successful authentication, Google provides the application with the required authentication information, and the user can access the application.

---

7. What is synchronous vs asynchronous communication?

Synchronous communication means the application waits for a response before continuing with the operation.

Asynchronous communication means the application can continue doing other work while waiting for a response.

Example

Synchronous:
Send request → Wait → Receive response

Asynchronous:
Send request → Continue other work → Receive response later

---

## 8. What is REST?

REST (Representational State Transfer) is an architectural style used for designing web APIs. REST APIs commonly use HTTP methods to perform operations on resources.

Example

GET /employees → Read employees

POST /employees → Create an employee

PUT /employees/1 → Update an employee

DELETE /employees/1 → Delete an employee
