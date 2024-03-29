# HTTP Method

[`GET`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET)

The `GET` method requests a representation of the specified resource. Requests using `GET` should only retrieve data.

The request parameter of the get method is appended to the URL.

Get request is better for the data which does not need to be secure (It means the data which does not contain images or word documents).

[`HEAD`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/HEAD)

The `HEAD` method asks for a response identical to a `GET` request, but without the response body.

[`POST`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST)

The `POST` method submits an entity to the specified resource, often causing a change in state or side effects on the server.

This data sent to the server is stored in the request body of the HTTP request.

It is not one of the most secure methods because the data that is been sent is included in the body of the request and not in the URL.&#x20;

Post request is better for the data which needs to be secure (It means the data which contains images or word documents).

[`PUT`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PUT)

The `PUT` method replaces all current representations of the target resource with the request payload.

[`DELETE`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/DELETE)

The `DELETE` method deletes the specified resource.

[`CONNECT`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/CONNECT)

The `CONNECT` method establishes a tunnel to the server identified by the target resource.

[`OPTIONS`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/OPTIONS)

The `OPTIONS` method describes the communication options for the target resource.

[`TRACE`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/TRACE)

The `TRACE` method performs a message loop-back test along the path to the target resource.

[`PATCH`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH)

The `PATCH` method applies partial modifications to a resource.
