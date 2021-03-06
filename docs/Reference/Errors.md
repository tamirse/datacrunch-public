# Errors

In addition to the standard HTTP status error codes, Error response contain data with the following schema:

Key | Info | 
---------|----------|
 code | Error type |
 message | Textual description of the error details |

 Error types:

Code | Description | Matching HTTP error code
---------|----------|----------|
 invalid_request | Invalid request, usually an input error - missing or invalid property etc. | 400 |
 unauthorized_request | Access token is missing or invalid  | 401 |
 insufficient_funds | Not enough funds to perform the action | 402 |
 forbidden_action | Can't perform the current action | 403 |
 not_found | Resource not found | 404 |
 server_error | Error on datacrunch's side | 500 |
 service_unavailable | Not enough resources at the moment, try again later | 503 |