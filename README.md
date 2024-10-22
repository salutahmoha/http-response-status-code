# http-response-status-code
### 1. Informational responses
- <p><b>100 Continue:</b> The server has received the request headers, and the client should proceed to send the request body.<p/>
- <p><b>101 Switching Protocols: </b>The requester has asked the server to switch protocols, and the server has agreed.</p>
- <p><b>102 Processing:</b>The server has received and is processing the request, but no response is available yet (WebDAV).</p>
- <p><b>103 Early Hints:</b>Used to return some headers before the final response.</p>
  
### 2. Successful responses
- <p><b>200 OK:</b>The request has succeeded.</p>
- <p><b>201 Created:</b>The request has been fulfilled and a new resource has been created.</p>
- <p><b>202 Accepted:</b>The request has been accepted for processing, but the processing is not complete.</p>
- <p><b>203 Non-Authoritative Information:</b>The request was successful but the returned meta-information comes from a third-party.</p>
- <p><b>204 No Content:</b>The request was successful, but there is no content to send back.</p>
- <p><b>205 Reset Content:</b>The server successfully processed the request, and asks the client to reset the document view.</p>
- <p><b>206 Partial Content:</b>The server is delivering only part of the resource due to a range header sent by the client.</p>
- <p><b>207 Multi-Status:</b>Provides status for multiple independent operations (WebDAV).</p>
- <p><b>208 Already Reported:</b>The members of a DAV binding have already been reported in a previous reply (WebDAV).</p>
- <p><b>226 IM Used: </b>The server has fulfilled a request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.</p>

### 3. Redirection messages
- <p><b>300 Multiple Choices: </b>The request has more than one possible response; user or agent must choose.</p>
- <p><b>301 Moved Permanently: </b>The URL of the requested resource has been permanently changed.</p>
- <p><b>302 Found:</b>Temporary redirect to another URL.</p>
- <p><b>303 See Other:</b>The server is redirecting to a different resource using a GET method.</p>
- <p><b>304 Not Modified:</b>The resource has not been modified since the last request.</p>
- <p><b>305 Use Proxy:</b>The requested resource must be accessed through the proxy given by the server.</p>
- <p><b>306 (Unused):</b>This code was used in previous versions, but is no longer in use.</p>
- <p><b>307 Temporary Redirect:</b>The requested resource temporarily resides at a different URL.</p>
- <p><b>308 Permanent Redirect: </b>The requested resource is now permanently located at a new URL.</p>

### 4. Client error messages
- <p><b>400 Bad Request:</b>The server cannot process the request due to malformed syntax.</p>
- <p><b>401 Unauthorized:</b>Authentication is required to access the resource.</p>
- <p><b>402 Payment Required:</b>Reserved for future use (initially intended for digital payment systems).</p>
- <p><b>403 Forbidden:</b>The server understands the request, but refuses to authorize it.</p>
- <p><b>404 Not Found:</b>The requested resource could not be found.</p>
- <p><b>405 Method Not Allowed:</b>The request method is not supported for the requested resource.</p>
- <p><b>406 Not Acceptable:</b>The requested resource is not available in a format that would be acceptable to the client.</p>
- <p><b>407 Proxy Authentication Required:</b>The client must authenticate with the proxy.</p>
- <p><b>408 Request Timeout:</b>The server timed out waiting for the request.</p>
- <p><b>409 Conflict:</b>The request conflicts with the current state of the server.</p>
- <p><b>410 Gone:</b>The resource requested is no longer available and will not be available again.</p>
- <p><b>411 Length Required:</b>The request did not specify the length of its content, which is required.</p>
- <p><b>412 Precondition Failed:</b>One or more conditions given in the request headers evaluated to false.</p>
- <p><b>413 Payload Too Large:</b>The request is larger than the server is willing or able to process.</p>
- <p><b>414 URI Too Long: </b>The URL provided was too long for the server to process.</p>
- <p><b>415 Unsupported Media Type:</b>The request's media format is not supported by the server.</p>
- <p><b>416 Range Not Satisfiable:</b>The client has asked for a portion of the file, but the server cannot supply that portion.</p>
- <p><b>417 Expectation Failed:</b>The server cannot meet the requirements of the Expect request-header field.</p>
- <p><b>418 I'm a teapot:</b>A joke status code defined in RFC 2324, "Hyper Text Coffee Pot Control Protocol."</p>
- <p><b>419 Page Expired: </b>Session or page has expired (often used in non-standard implementations).</p>
- <p><b>420 Enhance Your Calm:</b>Used by some sites (like Twitter) to indicate rate-limiting.</p>
- <p><b>421 Misdirected Request:</b>The request was directed at a server that cannot produce a response.</p>
- <p><b>422 Unprocessable Entity:</b>The request was well-formed but could not be followed due to semantic errors.</p>
- <p><b>423 Locked:</b>The resource that is being accessed is locked (WebDAV).</p>
- <p><b>424 Failed Dependency:</b>The request failed due to failure of a previous request (WebDAV).</p>
- <p><b>425 Too Early: </b>The server is unwilling to risk processing a request that might be replayed.</p>
- <p><b>426 Upgrade Required:</b>The client should switch to a different protocol.</p>
- <p><b>427 (Unused):</b>This status code is not used.</p>
- <p><b>428 Precondition Required:</b>The origin server requires the request to be conditional.</p>
- <p><b>429 Too Many Requests:</b>The user has sent too many requests in a given amount of time.</p>
- <p><b>430 (Unused): </b>This status code is not used.</p>
- <p><b>431 Request Header Fields Too Large: </b>The server is unwilling to process the request because the header fields are too large.</p>
- <p><b>451 Unavailable For Legal Reasons:</b>The resource cannot be served due to legal reasons (e.g., censorship).</p>

### 5. Server error responses
- <p><b>500 Internal Server Error: </b>General server error.</p>
- <p><b>501 Not Implemented: </b>The server does not support the request method.</p>
- <p><b>502 Bad Gateway: </b>Invalid response from an upstream server.</p>
- <p><b>503 Service Unavailable: </b>Server overloaded or under maintenance.</p>
- <p><b>504 Gateway Timeout: </b>Upstream server did not respond in time.</p>
- <p><b>505 HTTP Version Not Supported: </b>Server does not support the HTTP version used.</p>
- <p><b>506 Variant Also Negotiates: </b>Internal configuration error related to content negotiation.</p>
- <p><b>507 Insufficient Storage: </b>Server lacks storage space to complete the request (WebDAV).</p>
- <p><b>508 Loop Detected: </b>Infinite loop encountered during request processing (WebDAV).</p>
- <p><b>510 Not Extended: </b>Additional request extensions are required.</p>
- <p><b>511 Network Authentication Required: </b>Client must authenticate to access the network.</p>

