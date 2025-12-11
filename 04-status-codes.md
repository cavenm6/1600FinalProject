# **4. HTTP Status Codes**

HTTP status codes are three-digit numbers sent by a server in response to a client's request.  
They tell the client whether the request succeeded, failed, or requires additional action.

Status codes are grouped into **five major categories** based on their first digit.

---

## **1xx — Informational**
These codes indicate that the request was received and the server is continuing to process it.

Common examples:
- **100 Continue** — The server received request headers and the client should continue.
- **101 Switching Protocols** — The server is switching to a different protocol as requested.

---

## **2xx — Success**
These codes indicate the request was successfully processed.

Common examples:
- **200 OK** — Request succeeded; content is being returned.
- **201 Created** — A new resource has been created (commonly after a POST).
- **204 No Content** — Request succeeded but no data is returned.

---

## **3xx — Redirection**
The client must take further action, usually by making another request.

Common examples:
- **301 Moved Permanently** — The resource has a new permanent URL.
- **302 Found** — The resource is temporarily located elsewhere.
- **304 Not Modified** — The client can use a cached version of the resource.

---

## **4xx — Client Errors**
These occur when the client makes a bad request.

Common examples:
- **400 Bad Request** — The request was malformed.
- **401 Unauthorized** — Authentication is required.
- **403 Forbidden** — The server understands the request but refuses to authorize it.
- **404 Not Found** — The resource does not exist (most famous error on the web).

---

## **5xx — Server Errors**
These indicate the server failed to fulfill a valid request.

Common examples:
- **500 Internal Server Error** — The server encountered an unexpected issue.
- **502 Bad Gateway** — The server received an invalid response from an upstream server.
- **503 Service Unavailable** — The server is temporarily offline or overloaded.

---

## Why Status Codes Matter
- Help diagnose problems  
- Inform browsers how to react  
- Used heavily in APIs and debugging  
- Improve user experience (correct redirects, caching, etc.)

---

## Navigation
[Back: HTTP Responses](03-http-responses.md)  
[Next: Headers & Methods](05-headers-methods.md)

