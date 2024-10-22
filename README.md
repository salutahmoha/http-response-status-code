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
- <p><b>205 Reset Content:</b>The server successfully processed the request, and asks the client to reset the document view.
</p>
- <p><b>206 Partial Content:</b>The server is delivering only part of the resource due to a range header sent by the client.</p>
- <p><b>207 Multi-Status:</b>Provides status for multiple independent operations (WebDAV).
</p>
- <p><b>208 Already Reported:</b>The members of a DAV binding have already been reported in a previous reply (WebDAV).</p>
- <p><b>226 IM Used: </b>The server has fulfilled a request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.
</p>

### 3. Redirection messages
### 4. Client error messages
### 5. Server error responses
