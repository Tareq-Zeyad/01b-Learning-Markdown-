## **THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS**
### **Why Store Data**?
### *The main reason is practicality.*
### In the past a native client application was capable of storing data retrieving application-specific data like preferences or runtime state. Which was a advantage over web applications that did not have such luxury.
### So what we basically need :
### **a lot of storage space on the client that persists beyond a page refresh and isn’t transmitted to the server**

&lt;&gt;


### That the story before HTML5.
![html5](https://clementbuchanan.github.io/reading-notes/images/html5.jpg)

### So what is HTML5 Storage? A **Web Storage**. Simply, a way for web pages to store named key/value pairs locally, within the client web browser. **Like cookies**, this data remain even after you navigate away from the web site. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

&lt;&gt;

### **Html5 as a Storage platform**.
### HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

