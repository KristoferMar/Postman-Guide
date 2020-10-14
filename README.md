# Postman-Guide
Postman is a software development tool. It enables people to test calls to APIs. Postman users enter data. The data is sent to a special web server address. Typically, information is returned, which Postman presents to the user.

<h2>Tips and tricks</h2>

<h3>Autostore bearer token</h3>
You can automatically store a token for your REST requests the following way. <br>

1. Make sure you have an "Environment" registed for your project.
2. Find/create your "Login User" POST request for your backend and add the following line under the "Tests" tab. 
"pm.environment.set("TOKEN", pm.response.json().token)"
3. Save and make sure taht the environment variable "TOKEN" is created and stored under your "Environment quick look" tab whenever you execute a login requst. 
