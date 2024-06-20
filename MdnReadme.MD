

# HTTP Status Codes Overview

This document provides a  summary of HTTP status codes as defined in the MDN documentation. These codes indicate the result of an HTTP request.

## 1xx: Informational Responses
Informational status codes indicate that the request was received and understood, and the client should continue the request or ignore it if it is already finished.

- **100 Continue**: Request headers received; client should send the request body.
- **101 Switching Protocols**: Switching to the protocol requested by the client.
- **102 Processing (WebDAV)**: Request received and is being processed, no response yet.
- **103 Early Hints**: Final response likely to contain the header fields included in this response.

## 2xx: Success
These codes indicate that the request was successfully received, understood, and accepted.

- **200 OK**: Request succeeded; resource returned.
- **201 Created**: Request succeeded; new resource created.
- **202 Accepted**: Request accepted for processing, not complete.
- **203 Non-Authoritative Information**: Request succeeded; information from a third party.
- **204 No Content**: Request succeeded; no content to return.
- **205 Reset Content**: Request succeeded; client should reset the view.
- **206 Partial Content**: Partial content returned due to a range request.
- **207 Multi-Status (WebDAV)**: Multiple status codes for different parts of the message.
- **208 Already Reported (WebDAV)**: Members of a DAV binding already enumerated.
- **226 IM Used**: GET request fulfilled with instance-manipulations applied.

## 3xx: Redirection
Indicates that further action is needed to complete the request.

- **300 Multiple Choices**: Multiple possible responses; choose one.
- **301 Moved Permanently**: Resource permanently moved to a new URI.
- **302 Found**: Resource temporarily moved to a new URI.
- **303 See Other**: Response at a different URI, GET method used.
- **304 Not Modified**: Resource not modified since specified version.
- **305 Use Proxy (Deprecated)**: Access resource through a specified proxy.
- **306 Switch Proxy**: No longer used, reserved.
- **307 Temporary Redirect**: Resource temporarily under a different URI.
- **308 Permanent Redirect**: Resource permanently under a new URI.

## 4xx: Client Errors
These codes indicate that the request contains bad syntax or cannot be fulfilled.

- **400 Bad Request**: Request cannot be processed due to a client error.
- **401 Unauthorized**: Authentication required or failed.
- **402 Payment Required**: Reserved for future use.
- **403 Forbidden**: Server refuses to authorize the request.
- **404 Not Found**: Server cannot find the requested resource.
- **405 Method Not Allowed**: Method not supported for the resource.
- **406 Not Acceptable**: Resource generates only non-acceptable content.
- **407 Proxy Authentication Required**: Client must authenticate with the proxy.
- **408 Request Timeout**: Server timed out waiting for the request.
- **409 Conflict**: Conflict with the current state of the resource.
- **410 Gone**: Resource no longer available, no forwarding address.
- **411 Length Required**: Content length not specified, required by resource.
- **412 Precondition Failed**: Preconditions in request header not met.
- **413 Payload Too Large**: Request too large to be processed.
- **414 URI Too Long**: URI too long to be processed.
- **415 Unsupported Media Type**: Media type not supported.
- **416 Range Not Satisfiable**: Range request cannot be satisfied.
- **417 Expectation Failed**: Expectation in request header cannot be met.
- **418 I'm a teapot**: Humorously indicates the server is a teapot.
- **421 Misdirected Request**: Request directed at an inappropriate server.
- **422 Unprocessable Entity (WebDAV)**: Well-formed request, but semantic errors.
- **423 Locked (WebDAV)**: Resource is locked.
- **424 Failed Dependency (WebDAV)**: Failed due to previous request failure.
- **425 Too Early**: Request might be replayed.
- **426 Upgrade Required**: Client should use a different protocol.
- **428 Precondition Required**: Request must be conditional.
- **429 Too Many Requests**: Too many requests in a given time period.
- **431 Request Header Fields Too Large**: Header fields too large to process.
- **451 Unavailable For Legal Reasons**: Access denied due to legal demand.

## 5xx: Server Errors
These codes indicate that the server failed to fulfill a valid request.

- **500 Internal Server Error**: Generic error, unexpected condition.
- **501 Not Implemented**: Request method not supported.
- **502 Bad Gateway**: Invalid response from upstream server.
- **503 Service Unavailable**: Server not ready to handle the request.
- **504 Gateway Timeout**: No timely response from upstream server.
- **505 HTTP Version Not Supported**: HTTP protocol version not supported.
- **506 Variant Also Negotiates**: Circular reference in content negotiation.
- **507 Insufficient Storage (WebDAV)**: Not enough storage to complete request.
- **508 Loop Detected (WebDAV)**: Infinite loop detected in request processing.
- **510 Not Extended**: Further extensions required to fulfill request.
- **511 Network Authentication Required**: Client needs network authentication.