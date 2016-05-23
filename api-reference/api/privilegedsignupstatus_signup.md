# privilegedSignupStatus: signUp
Sign up the tenant to Privileged Identity Management.

### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Global Administrator_ role. 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedSignupStatus/signUp
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body

### Response
If successful, this method returns `200, OK` response code and [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_signup"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedSignupStatus/signUp
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedSignupStatus"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 74

{
  "id": "id-value",
  "isRegistered": true,
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSignupStatus: signUp",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->