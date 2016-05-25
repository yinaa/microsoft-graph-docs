# privilegedRoleAssignment: makeTemporary
Make the permanent role assignment as temporary. The role will be set as active with the default expiration time.

### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_


The requestor needs to have _Privileged Role Administrator_ role. 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/<id>/makeTemporary
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns `200, OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_maketemporary"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/<id>/makeTemporary
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "datetime-value",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makeTemporary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->