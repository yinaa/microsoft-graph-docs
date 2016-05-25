# privilegedSecurityAlert: fix

Fix the issues that trigger the alert.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Privileged Role Administrator_ role.
 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedSecurityAlerts/<id>/fix
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|itemId|int32|Optional. The id of the item that triggers the alert and the request intends to fix.  If the value is not specified, the service will fix all issue items that trigger the alert.|

### Response
If successful, this method returns `200, OK` response code.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsecurityalert_fix"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedSecurityAlerts/<id>/fix
Content-type: application/json
Content-length: 18

{
  "itemId": 99
}
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
  "description": "privilegedSecurityAlert: fix",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->