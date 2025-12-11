# **3. HTTP Responses**

An **HTTP response** is the message a server sends back to a client after receiving and processing an HTTP request.  
It contains the requested resource (if available) and important information describing the result of the request.

Every time your browser loads a webpage, it is processing one or more HTTP responses.

---

## Structure of an HTTP Response

An HTTP response has three main parts:

---

### **1. Status Line**
This includes:
- The HTTP version  
- A **status code** (e.g., 200, 404, 500)  
- A short message describing the code  

Example:
HTTP/1.1 200 OK


---

### **2. Headers**
Response headers provide additional information about the returned content.

Examples:
Content-Type: text/html
Content-Length: 5120
Set-Cookie: sessionID=12345


Common response headers include:
- **Content-Type** (HTML, JSON, image, etc.)  
- **Content-Length** (size of the response body)  
- **Set-Cookie** (stores data on the client)  
- **Server** (information about the server software)

---

### **3. Body**
The body is the actual content being returned.  
This might be:
- An HTML page  
- An image  
- JSON data  
- A file  
- An error message  

Example body (HTML):

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Welcome!</h1>
  </body>
</html>

HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 137

<!DOCTYPE html>
<html>
  <body>
    <h1>Hello World</h1>
  </body>
</html>

## How Requests and Responses Work Together
### **Client → Server (Request)**

GET /home HTTP/1.1  
Host: example.com  
User-Agent: Chrome/123.0  
Accept: text/html  

### **Server → Client (Response)**

HTTP/1.1 200 OK  
Content-Type: text/html  
Content-Length: 52  

<!DOCTYPE html>
<html>
  <body>
    <h1>Home Page</h1>
  </body>
</html>

## 📎 Navigation
[Back: HTTP Requests](02-http-requests.md)  
[Next: HTTP Status Codes](04-status-codes.md)
