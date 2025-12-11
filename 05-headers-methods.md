# **5. HTTP Headers & Methods**

HTTP headers and methods provide essential information about how clients and servers communicate.  
They control everything from browser identity to content formatting, cookies, caching, and how data is sent.

---

# Part 1: HTTP Headers

HTTP headers are key–value pairs included in both **requests** and **responses**.  
They give extra details about the message, such as content type, language, cookies, and more.

---

## Common Request Headers

| Header | Purpose |
|--------|----------|
| **Host** | Identifies the domain being requested |
| **User-Agent** | Identifies the browser or application |
| **Accept** | Lists content types the client can handle |
| **Authorization** | Sends login credentials or tokens |
| **Cookie** | Sends stored data from previous sessions |

**Example request headers:**
Host: example.com
User-Agent: Chrome/123.0
Accept: text/html
Cookie: sessionID=12345


---

## Common Response Headers

| Header | Purpose |
|--------|----------|
| **Content-Type** | Describes the type of returned data (HTML, JSON, image, etc.) |
| **Content-Length** | Size of the returned body |
| **Set-Cookie** | Stores data on the client (used for sessions) |
| **Server** | Information about the server software |
| **Cache-Control** | Tells the browser how to cache the response |

**Example response headers:**
Content-Type: text/html
Content-Length: 5120
Set-Cookie: sessionID=12345
Server: nginx


---

# Part 2: HTTP Methods (Detailed)

HTTP methods define **what action** the client wants to perform on a resource.

---

## **GET**
- Requests a resource  
- Should **not** change server data  
- Most common method  
- No request body  

Example:
GET /home HTTP/1.1


---

## **POST**
- Sends data to the server  
- Common for forms, login, uploading data  
- Often changes server state  

Example:
POST /login HTTP/1.1
Content-Type: application/x-www-form-urlencoded

username=admin&password=1234

---

## **PUT**
- Updates or replaces an existing resource  
- Often used in APIs  

---

## **DELETE**
- Removes a resource from the server  

---

## **HEAD**
- Same as GET, but returns **only headers**  
- Useful for checking resource size or availability  

---

## **PATCH**
- Partially updates a resource  
- More efficient than PUT for small edits  

---

# Summary
- **Headers** carry important metadata with every request and response  
- **Methods** define the action the client wants to perform  
- Understanding these concepts is essential for working with APIs, web servers, and modern applications  

---

## Navigation
[Back: HTTP Status Codes](04-status-codes.md)  
[Next: End-to-End Example](06-http-example.md)
