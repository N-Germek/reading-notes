# CRUD Beginings

## Status Codes Based on Rest Methods

In your own words, describe what each group of status code represents:

100’s = Informational status codes that tell the cleint that the header request has been received and the server will try to comply.

200’s = Success codes stating the request was accepted and that they have met validation requirements at the time they were sent.

300’s = Redirection codes for client request that tell the client the requested URL is not in the search location and if available, where the new URL is located. These can be temporary or permanent.

400’s = Cleint error codes for invalid requests for many reasons including incorrect URL, missing authenticvation, timeouts etc.

500’s = Server error codes, commonly caused by overwhelmed servers or unreachable servers behind proxies. Sometimes they can be returned from a client request that trigger error exceptions. These also can be temporary or permanent and would require the client to resubmit the request.

What is a status code 202? This is the asynchronous processinng request that means all validation requirements were met at the time of sending yet it wasn't successfully processed.

What is a status code 308? This is a permanent redirect code that tells the client to use another URL for access to that resource.

What code would you use if an update didn’t return data to a client?
Code 204 No Content.

What code would you use if a resource used to exist but no longer does?
Code 410 Gone.

What is the ‘Forbidden’ status code?
Code 403 is the forbidden status code for instances where the client does not have access to the resource.

- > [Table Of Contents](READING-NOTES/README.md)

- > [Home Page](README.md)

## Things I want to learn more about:

### Resources

- > [Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

- > [Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)
