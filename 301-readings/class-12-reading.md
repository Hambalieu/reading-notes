# Readings: CRUD
<br></br>

## Status Codes Based On REST Methods<br></br>
## In your own words, describe what each group of status code represents:
- 100’s = These are informational status codes
- 200’s = These are the success codes. They tell the client that its request was accepted
- 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore
- 400’s = These are the client error codes. They are all about invalid requests a client sent to a server
- 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server.

## What is a status code 202?
- Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.

## What is a status code 308?
- This tells the client to use another URL to access the resource and not use the current URL anymore

## What code would you use if an update didn’t return data to a client?
- 204 No Content

## What code would you use if a resource used to exist but no longer does?
- 410 Gone

## What is the ‘Forbidden’ status code?
- 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.<br></br>


## Build A REST API With Node.js, Express, & MongoDB - Quick .<br></br>

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- Because when we deploy our app we dont want to use our local host.

## What is middleware?
- Is the code that runs when the server gets a resquest but before it get passed to our routes.

## What does app.use(express.json()) do?
- it allows our server to accept json as a body for request
## What does the /:id mean in a route?
-  it means that its a parameter request

## What is the difference between PUT and PATCH?
- PUT updates all the information all at once while  PATCH only updates what the user passes us.

## How do you make a default value in a schema?
- default: 
- by using the word defaul in our object property
## What does a 500 error status code mean?
-  These are the server error codes.

## What is the difference between a status 200 and a status 201?
- **200 OK** - It’s the basic status code to tell the client everything went good while **201 Created**- The most fitting for Create operations

<br></br>

## References/Citations
[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)<br></br>
[Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)


