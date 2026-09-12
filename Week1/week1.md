## 1. GET Request

### Command

    curl -i https://api.github.com/users/torvalds

### Status Code

*200 OK*

The request was successful.

### Response Headers

1. *Content-Type* - Shows the format of the response.
2. *Cache-Control* - Gives information about caching the response.
3. *ETag* - Identifies a version of the response.

### Response Body

The response contains GitHub user information such as username, name, location, followers and public repositories.

### Observation

I used a GET request to retrieve the details of a GitHub user. The server returned 200 OK and the data was returned in JSON format.

---

## 2. Verbose GET Request

### Command

    curl -v https://httpbin.org/get

### Status Code

*200 OK*

The request was successful.

### Response Headers

1. *Content-Type* - Shows the response format.
2. *Content-Length* - Shows the size of the response.
3. *Server* - Shows the server software.

### Response Body

The response contains information about the request, such as headers, origin and URL.

### Observation

I used the verbose curl command to see more details about the request and response. It showed the connection details and response information.

---

## 3. POST Request

### Command

    curl -i -X POST https://httpbin.org/post \
    -H "Content-Type: application/json" \
    -d '{"name":"Prakash","week":1}'

### Status Code

*200 OK*

The request was successful.

### Response Headers

1. *Content-Type* - Shows the format of the response.
2. *Content-Length* - Shows the size of the response.
3. *Server* - Shows the server software.

### Response Body

The response contains the JSON data that I sent to the server.

### Observation

I used a POST request to send JSON data to the server. The server received the JSON data and returned it in the response.

---

## 4. Query Parameters

### Command

    curl -i "https://httpbin.org/get?role=intern&track=java"

### Status Code

*200 OK*

The request was successful.

### Query Parameters

- *role=intern* - Specifies the role as intern.
- *track=java* - Specifies Java as the learning track.

### Response Body

The response contains the query parameter values that were sent through the URL.

### Observation

I used query parameters to send additional information through the URL. The server returned the values in the response.

---

## 5. Non-Existing User

### Command

    curl -i https://api.github.com/users/this-user-does-not-exist-99999

### Status Code

*404 Not Found*

The requested user was not found.

### Response Body

The response contains an error message because the requested GitHub user does not exist.

### Observation

I requested a GitHub user that does not exist. The server returned 404 Not Found because the requested resource was unavailable.

---

# Postman Verification

## GET Request

I sent the same GET request using Postman.

### Result

- *Method:* GET
- *Status Code:* 200 OK
- *Response:* GitHub user information was returned successfully.

## POST Request

I sent the same POST request using Postman with JSON data.

### Result

- *Method:* POST
- *Status Code:* 200 OK
- *Response:* The JSON data was returned successfully.

### Observation

Postman helped me verify the API requests and responses. I confirmed the status codes and response data.
