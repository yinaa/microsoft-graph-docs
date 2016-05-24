# privilegedRoleAssignment: uniqueAdminsCount
Use this API to get the number of unique administrators that have the privileged roles assigned.

### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.  
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/<id>/uniqueAdminsCount
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body

### Response
If successful, this method returns `200, OK` response code and int32 object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_uniqueadminscount"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/<id>/uniqueAdminsCount
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 17

{
  "value": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: uniqueAdminsCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
