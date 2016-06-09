# privilegedOperationEvent resource type

Represents an audit event that is generated for the role operations, such as an administrator manages privileged roles, and a user activates/deactivates his roles.


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent_list.md) | [privilegedOperationEvent](privilegedoperationevent.md) collection. |Get collection of privilegedOperationEvent objects.|
|[Create](../api/privilegedoperationevent_post_privilegedoperationevents.md) | [privilegedOperationEvent](privilegedoperationevent.md)	|Create privilegedOperationEvent object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|additionalInformation|string|Detailed human readable information for the event.|
|creationDateTime|dateTimeOffset|Indicates the time when the event is created.|
|expirationDateTime|dateTimeOffset|This is only used when the requestType is "Elevate", and it indicates the expiration time for the role activation.|
|id|string|The unique identifier for privilegedOperationEvent. Read-only.|
|requestType|string|The request operation type. Example types could be: Assign (role assignment), Elevate (role activation), Unassign (remove role assignment), and Unelevate (role deactivation).|
|requestorId|string|The user id of the requestor who initiates the operation.|
|requestorName|string|The user name of the requestor who initiates the operation.|
|roleId|string|The id of of the role that is associated with the operation.|
|roleName|string|The name of the role.|
|tenantId|string|The tenant(organization) id.|
|userId|string|The id of the user that is associated with the operation.|
|userMail|string|The user's email.|
|userName|string|The user's display name.|

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
