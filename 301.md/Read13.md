## **CRUD.**
## **Status Codes Based On REST Methods.**

- ### *In your own words, describe what each group of status code represents:*
- ### **100's:** These are informational status codes; they usually tell the client that the header part of the request has been received.
- ### **200's:** These are the success codes. They tell the client that a request was accepted
- ### **300's:** These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. 
- ### **400's:** These are the client error codes. They are all about invalid requests a client sent to a server.
- ### **500's:** These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies.
<br>

- ### *What is a status code 202?*
### This code tells the client that the request was valid, but its processing will finish sometime in the future.
<br>

- ### *What is a status code 308?*
### This tells the client to use another URL to access the resource and not use the current URL anymore.
<br>

- ### *What code would you use if an update didn’t return data to a client?*
### 204 No Content.
<br>

- ### *What code would you use if a resource used to exist but no longer does?*
###  410.
<br>

- ### *What is the ‘Forbidden’ status code?*
### 403.
<br>

## **Build A REST API With Node.js, Express, & MongoDB - Quick**
- ### *Why do we need to pull our MongoDB database string out of our server and put it into our .env?*
### when we want to deploy our applcation we dont want to use localhost in it.
<br>

- ### *What is middleware?*
### code that runs when the server get request but before passed route
<br>

- ### *What does app.use(express.json()) do?*
### accept the json file and use it.
<br>

- ### *What does the /:id mean in a route?*
###  It does: req.params.id
<br>

- ### *What is the difference beween PUT and PATCH?*
### PUT is a method of modifying resource where the client sends data that updates the entire resource.
<br>

- ### *How do you make a defalut value in a schema?*
### use default : Date.now
<br>

- ### *What does a 500 error status code mean?*
### error in the server
<br>

- ### *What is the difference between a status 200 and a status 201?*
### 200: the request was received and understood and is being processed. 201: a request was successful and as a result, a resource has been created.
<br>