# privilegedSignupStatus resource type

Represents the organization sign-up status for Privileged Identity Management.


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[List privilegedSignupStatus](../api/privilegedsignupstatus_list.md) | [privilegedSignupStatus](privilegedsignupstatus.md) |Read properties and relationships of privilegedSignupStatus object.|
|[canSignUp](../api/privilegedsignupstatus_cansignup.md)|boolean|Verify if the requestor is authorized to sign up the organization to Privileged Identity Management.|
|[completeSetup](../api/privilegedsignupstatus_completesetup.md)|[roleSuccessStatistics](rolesuccessstatistics.md) collection|Finish Privileged Identity Management sign up process with the organization administrator specified parameters.|
|[isSignedUp](../api/privilegedsignupstatus_issignedup.md)|boolean|Check if the organization is signed up to Privileged Identity Management.|
|[signUp](../api/privilegedsignupstatus_signup.md)|[privilegedSignupStatus](privilegedsignupstatus.md)|Start the sign up process to Privileged Identity Management for the organization.|

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|id|string| Read-only.|
|isRegistered|boolean|**true** if the organization has initiated PIM registration. **false** if the organization has not initiated PIM registration or if the previous registration was failed.|
|status|string| Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedSignupStatus"
}-->

```json
{
  "id": "string (identifier)",
  "isRegistered": true,
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSignupStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
