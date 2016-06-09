# tenantSetupInfo resource type

Represents the tenant setup information, which is used as the passed in parameter by [completeSetup](../api/privilegedsignupstatus_completesetup.md) method.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|firstTimeSetup|boolean|**true** if it's the first time for the tenant to sign up PIM. **false** otherwise.|
|id|string| The unique identifier. Read-only.|
|relevantRolesSettings|string collection|A collection of role IDs that method completeSetup will configure the role settings to.|
|setupStatus|string| Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|
|skipSetup|boolean|**true** if skip setup process when running completeSetup method. **false** if need to run setup process when running completeSetup method.|
|userRolesActions|string|Contains a list of user to role assignment action items. Each action item is in the format of "userId &#124; roleId &#124; Action". The action items are separated by semicolon (;). For example: "163f4c90-c165-4f8c-913d-de12c3884f90 &#124; 62e90394-69f5-4237-9190-012177145e10&#124;Permanent;28d63d00-2d64-41d9-8ff6-ad56e3f8bf21&#124;62e90394-69f5-4237-9190-012177145e10&#124;Temporary"|

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|defaultRolesSettings|[privilegedRoleSettings](privilegedrolesettings.md)| Read-only. Nullable. Contains the default role settings, including the role activation duration, is MFA required during role activation, and if need to notify the user when the user role is activated.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tenantSetupInfo"
}-->

```json
{
  "firstTimeSetup": true,
  "id": "string (identifier)",
  "relevantRolesSettings": ["string"],
  "setupStatus": "string",
  "skipSetup": true,
  "userRolesActions": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tenantSetupInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->