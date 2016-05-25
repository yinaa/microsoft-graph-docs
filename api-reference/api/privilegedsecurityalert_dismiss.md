# privilegedSecurityAlert: dismiss
Dismiss the specified alert.

### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Privileged Role Administrator_ role.
 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedSecurityAlerts/<id>/dismiss
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns `200, OK` response code and [privilegedSecurityAlert](../resources/privilegedsecurityalert.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsecurityalert_dismiss"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedSecurityAlerts/<id>/dismiss
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedSecurityAlert"
} -->
```http
HTTP/1.1 200 OK
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSecurityAlert: dismiss",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->