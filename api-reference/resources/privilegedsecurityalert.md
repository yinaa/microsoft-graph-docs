# privilegedSecurityAlert resource type

Represents the security alert object.


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[List](../api/privilegedsecurityalert_list.md) | Collection of [privilegedSecurityAlert](privilegedsecurityalert.md) |Get the collection of privilegedSecurityAlert objects. |
|[Get privilegedSecurityAlert](../api/privilegedsecurityalert_get.md) | [privilegedSecurityAlert](privilegedsecurityalert.md) |Read properties and relationships of privilegedSecurityAlert object.|
|[Update](../api/privilegedsecurityalert_update.md) | [privilegedSecurityAlert](privilegedsecurityalert.md)	|Update the properties for the privilegedSecurityAlert object. |
|[dismiss](../api/privilegedsecurityalert_dismiss.md)|[privilegedSecurityAlert](privilegedsecurityalert.md)|Dismiss the activated security alert so that it doesn't show up.|
|[fix](../api/privilegedsecurityalert_fix.md)|[privilegedSecurityAlert](privilegedsecurityalert.md)|Request the backend service to resolve the security alert by making the corresponding privileged role assignment changes.|
|[reactivate](../api/privilegedsecurityalert_reactivate.md)|[privilegedSecurityAlert](privilegedsecurityalert.md)|Activate the dismissed security alert so that the alert can show up in the management portal and the administrator is able to fix the issues that cause the security alert. |
|[refreshAll](../api/privilegedsecurityalert_refreshall.md)|[privilegedSecurityAlert](privilegedsecurityalert.md)|Request the backend service to scan the security alerts again and update the result.|

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|additionalData|string|The value is in a JSON format. It contains an array of items that trigger the security alert. For example: ```[{"ItemId":0,"RoleDisplayName":"Global Administrator","RoleId":"62e90394-69f5-4237-9190-012177145e10"},{"ItemId":1,"RoleDisplayName":"Exchange Administrator","RoleId":"29232cdf-9323-42fd-ade2-1d097af3e4de"},{"ItemId":2,"RoleDisplayName":"Billing Administrator","RoleId":"b0f54661-2d74-4c50-afa3-1ec803f12efe"}]```|
|alertDescription|string|A description message for the alert.|
|alertName|string|The name of the alert.|
|alertType|string| Possible values are: `vulnerability`, `attackSuspect`.|
|howToPrevent|string|The help message of how to prevent this security alert.|
|id|string| The unique identifier of the security alert. Read-only.|
|isActive|boolean|**true** if the security alert is active. **false** if the security alert is not active.|
|isConfigurable|boolean|**true** if the tenant administrator is able to configure the security alert. **false** if the security alert cannot be configured. |
|isResolvable|boolean|**true** if the security alert can be resolved running **fix** method. **false** if the security alert cannot be resolved by **fix** method. |
|lastModifiedDateTime|dateTimeOffset|The last modified time for the security alert.|
|lastScannedDateTime|dateTimeOffset|The last scanned time for the security alert.|
|mitigationSteps|string|Mitigate steps for the security alert.|
|numberOfAffectedItems|int32|The number of items that are affected by the security alert. The items are stored in **additionalData** property.|
|securityImpact|string|The help message of the security impact from the security alert.|
|severityLevel|string| Possible values are: `high`, `medium`, `low`.|
|status|string| Possible values are: `active`, `dismissed`, `inactive`.|
|wasDismissed|boolean|**true** if the security alert is dismissed by the tenant administrator. **false** if the security alert is not dismissed.|

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedSecurityAlert"
}-->

```json
{
  "additionalData": "string",
  "alertDescription": "string",
  "alertName": "string",
  "alertType": "string",
  "howToPrevent": "string",
  "id": "string (identifier)",
  "isActive": true,
  "isConfigurable": true,
  "isResolvable": true,
  "lastModifiedDateTime": "String (timestamp)",
  "lastScannedDateTime": "String (timestamp)",
  "mitigationSteps": "string",
  "numberOfAffectedItems": 1024,
  "securityImpact": "string",
  "severityLevel": "string",
  "status": "string",
  "wasDismissed": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSecurityAlert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->