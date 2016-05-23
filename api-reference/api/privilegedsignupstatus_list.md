# List privilegedSignupStatus

Retrieve the privilegedSignupStatus object for the tenant.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedSignupStatus
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer <code>|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedsignupstatus"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedSignupStatus
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedSignupStatus",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 115

{
  "value": [
    {
      "id": "id-value",
      "isRegistered": true,
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedSignupStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->