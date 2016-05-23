# Create privilegedOperationEvent

Use this API to create a new privilegedOperationEvent.
### Prerequisites
Only Azure AD Access Reviews service is able to call this API.
 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedOperationEvents
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body
In the request body, supply a JSON representation of [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.


### Response
If successful, this method returns `201, Created` response code and [privilegedOperationEvent](../resources/privilegedoperationevent.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedoperationevent_from_privilegedoperationevents"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedOperationEvents
Content-type: application/json
Content-length: 154

{
  "userId": "userId-value",
  "userName": "userName-value",
  "userMail": "userMail-value",
  "roleId": "roleId-value",
  "roleName": "roleName-value"
}
```
In the request body, supply a JSON representation of [privilegedOperationEvent](../resources/privilegedoperationevent.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "id-value",
  "userId": "userId-value",
  "userName": "userName-value",
  "userMail": "userMail-value",
  "roleId": "roleId-value",
  "roleName": "roleName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create privilegedOperationEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->