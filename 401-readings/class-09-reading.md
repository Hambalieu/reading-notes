# Read: 09 - WRRC and Java

### HttpUrlConnection
- The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries.
- The disadvantages of using this method are that the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication.

###Creating a Request
-The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: **GET**, **POST**, **HEAD**, **OPTIONS**, **PUT**, **DELETE**, **TRACE**.
>URL url = new URL("http://example.com");
HttpURLConnection con = (HttpURLConnection) url.openConnection();
con.setRequestMethod("GET");

###Configuring Timeouts
- These values define the interval of time to wait for the connection to the server to be established or data to be available for reading.
-To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() methods:
> con.setConnectTimeout(5000);
con.setReadTimeout(5000);

###Notes
- To read the cookies from a response, we can retrieve the value of the Set-Cookie header and parse it to a list of HttpCookie objects:
- To add the cookies to the request, we need to set the Cookie header, after closing and reopening the connection:
- It is also possible to enable or disable automatic redirect for all connections:
-To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods:
>int status = con.getResponseCode();
-To close the connection, we can use the disconnect() method:
> con.disconnect();
- 

## Reference and Citation
[Do a Simple HTTP Request in Java](https://www.baeldung.com/java-http-request)
[The HTTP Request Lifecycle](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)