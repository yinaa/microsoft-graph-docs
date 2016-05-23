# roleSuccessStatistics resource type
Represents the statistics summary for the privileged role assignments that are done during tenant sign up process to Privileged Identity Management.

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|permanentFail|int64|The number of failed permanent role assignments. |
|permanentSuccess|int64|The number of succeeded permanent role assignments. |
|removeFail|int64|The number of failed actions removing the role assignment.|
|removeSuccess|int64|The number of succeeded actions removing the role assignment.|
|roleId|string|The role id.|
|roleName|string|The role name.|
|temporaryFail|int64|The number of failed temporary role assignments.|
|temporarySuccess|int64|The number of succeeded temporary role assignments.|
|unknownFail|int64|The number of unknown failures.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roleSuccessStatistics"
}-->

```json
{
  "permanentFail": 1024,
  "permanentSuccess": 1024,
  "removeFail": 1024,
  "removeSuccess": 1024,
  "roleId": "string",
  "roleName": "string",
  "temporaryFail": 1024,
  "temporarySuccess": 1024,
  "unknownFail": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleSuccessStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->