# **2. HTTP Requests**

An **HTTP request** is a message sent from a client (such as a web browser) to a server. It asks for a resource—like a webpage, image, or data—and includes information that helps the server understand what the client wants.

Every time you:
- Type a URL  
- Click a link  
- Submit a form  
- Load an image  

…your device sends an HTTP request.

---

## Structure of an HTTP Request

A typical request includes three main parts:

### **1. Request Line**
This contains:
- The **method** (e.g., GET, POST)  
- The **path** (resource being requested)  
- The **HTTP version**

Example:
GET /index.html HTTP/1.1

---

### **2. Headers**
Headers provide additional information such as:
- Browser type  
- Preferred languages  
- Cookies  
- Accepted content formats  

Example:
Host: example.com
User-Agent: Chrome/123.0
Accept: text/html


---

## Navigation
[Back: What Is HTTP?](01-what-is-http.md)  
[Next: HTTP Responses](03-http-responses.md)

