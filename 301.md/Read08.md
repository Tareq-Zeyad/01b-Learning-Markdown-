## **API's**
### **API Design Best Practices**
<br>

- ### *What does REST stand for?*
### Representational State Transfer
<br>

- ### *REST APIs are designed around a ____.*
### resources, which are any kind of object, data, or service that can be accessed by the client.
<br>

- ### *What is an identifer of a resource?*
### A URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:HTTPhttps://adventure-works.com/orders
<br>

- ### *What are the most common HTTP verbs?*
### The most common operations are GET, POST, PUT, PATCH, and DELETE.
<br>

- ### *What should the URIs be based on?*
### URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
<br>

- ### *Give an example of a good URI.*
### (https://adventure-works.com/orders)
<br>

- ### *What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?*
### Expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires Its a bad thing.
<br>

- ### *What status code does a successful GET request return?*
### A successful GET method typically returns HTTP status code 200 (OK).
<br>

- ### *What status code does an unsuccessful GET request return?*
### If the resource cannot be found, the method should return 404 (Not Found).
<br>

- ### *What status code does a successful POST request return?*
### It returns HTTP status code 201 (Created).
<br>

- ### *What status code does a successful DELETE request return?*
### the web server should respond with HTTP status code 204 (No Content).