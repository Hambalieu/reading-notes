# Readings: API's
## What does REST stand for?
-In 2000, Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP.
</br></br>

## REST APIs are designed around a ____.
- resources, which are any kind of object, data, or service that can be accessed by the client.
</br></br>

## What is an identifer of a resource? Give an example.
- A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: 
  > https://adventure-works.com/orders/1

</br></br>

## What are the most common HTTP verbs?
- the most common are: GET, POST, PUT, PATCH, and DELETE.

</br></br>

## What should the URIs be based on?

- URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

</br></br>


## Give an example of a good URI.
- > https://adventure-works.com/orders 

</br></br>

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- its bad because Such an API may require a client application to send multiple requests to find all of the data that it requires.try to avoid it 

</br></br>

## What status code does a successful GET request return?
- GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource

</br></br>

## What status code does an unsuccessful GET request return?
- POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.

</br></br>

## What status code does a successful POST request return?
- PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.

</br></br>

## What status code does a successful PATCH request return?
- PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.

</br></br>

## What status code does a successful DELETE request return?
- DELETE removes the resource at the specified URI.

</br></br>

## Things I want to know more about
- I want to learn more about RegExr.


## How would you match a phone number from your city using RegEx?

-  ` /(\+\d{1,3}\s?)?((\(\d{3}\)\s?)|(\d{3})(\s|-?))(\d{3}(\s|-?))(\d{4})(\s?(([E|e]xt[:|.|]?)|x|X)(\s?\d+))?/gm`

    `test string : 2062124763`

</br></br>

## References/Citations

[API's](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
</br></br>


[RegExr](https://regexr.com/)

[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)

[Regex 101](https://regex101.com/)
