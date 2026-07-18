# HTTP Methods, Codes and more

## HTTP Requests 

### GET

The GET HTTP method requests a representation of the specified resource. Requests using GET should only be used to request data and shouldn't contain a body.

### POST

The POST HTTP method sends data to the server. The type of the body of the request is indicated by the Content-Type header. 

### PUT

The PUT HTTP method creates a new resource or replaces a representation of the target resource with the request content.

```
The difference between PUT and POST is that PUT is idempotent: calling it once is no different from calling it several times successively (there are no side effects).
```

### PATCH

The PATCH HTTP method applies partial modifications to a resource. PATCH request may not always be idempotent

```
In comparison with PUT, a PATCH serves as a set of instructions for modifying a resource, whereas PUT represents a complete replacement of the resource.
```

### DELETE

The DELETE HTTP method asks the server to delete a specified resource. Requests using DELETE should only be used to delete data and shouldn't contain a body.

