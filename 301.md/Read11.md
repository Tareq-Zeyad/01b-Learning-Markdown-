## **Authentication.**
## **What is OAuth.**

- ### *What is OAuth?*
### A JS library, OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.
<br>

- ### *Give an example of what using OAuth would look like.*
### The feature of log in, sign up to save to allow access to authorize users to use the service or app.
<br>

- ### *How does OAuth work? What are the steps that it takes to authenticate the user?*
- ### The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- ### The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- ### The first site gives this token and secret to the initiating user’s client software.
- ### The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- ### If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website. 
- ### The user approves (or their software silently approves) a particular transaction type at the first website.
- ### The user is given an approved access token (notice it’s no longer a request token).
- ### The user gives the approved access token to the first website.
- ### The first website gives the access token to the second website as proof of authentication on behalf of the user.
- ### The second website lets the first website access their site on behalf of the user.
- ### The user sees a successfully completed transaction occurring.
<br>

- ### *What is OpenID?*
### OpenID is for humans logging into machines
<br>

## **Authorization and Authentication flows**
- ### *What is the difference between authorization and authentication?*
### Authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.
<br>

- ### *What is Authorization Code Flow?*
### Which exchanges an Authorization Code for a token. Your app must be server-side because during this exchange, you must also pass along your application’s Client Secret, which must always be kept secure, and you will have to store it in your client.
<br>

- ### *What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?*
### The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier. 
<br>

- ### *What is Implicit Flow with Form Post?*
###  The intend for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.
<br>

- ### *What is Client Credentials Flow?*
### With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don’t make sense. Instead, M2M apps use the Client Credentials Flow.
<br> 

- ### *What is Device Authorization Flow?*
### With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.
<br>

- ### *What is Resource Owner Password Flow?*
### Requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.
<br>

## **Things I want to learn more about:**
### 1- The diference between SQL & noSQL.
### 2- The correct way to use Auth0.
