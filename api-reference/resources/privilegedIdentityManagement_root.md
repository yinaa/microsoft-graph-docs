# Service root


### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Create privilegedOperationEvent](../api/privilegedoperationevent_post_privilegedoperationevents.md) |[privilegedOperationEvent](privilegedoperationevent.md)| Create a new privilegedOperationEvent by posting to the privilegedOperationEvents collection.|
|[List privilegedOperationEvent](../api/privilegedoperationevent_list.md) | [privilegedOperationEvent](privilegedoperationevent.md) collection |Get privilegedOperationEvent object collection. |
|[Get privilegedRole](../api/privilegedrole_get.md) |[privilegedRole](privilegedrole.md)| Get a privilegedRole object.|
|[List privilegedRole](../api/privilegedrole_list.md) | [privilegedRole](privilegedrole.md) collection |Get privilegedRole object collection. |
|[List role assignments](../api/privilegedrole_list_assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection |Get privilegedRoleAssignment collection. |
|[selfActivate](../api/privilegedrole_selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Activate the role that is assigned to the requestor.|
|[selfDeactivate](../api/privilegedrole_selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Deactivate the role that is assigned to the requestor.|
|[Create privilegedRoleAssignment](../api/privilegedroleassignment_post_privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Create a new privilegedRoleAssignment by posting to the privilegedRoleAssignments collection.|
|[List privilegedRoleAssignment](../api/privilegedroleassignment_list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection |Get privilegedRoleAssignment object collection. |
|[Get privilegedRoleAssignment](../api/privilegedroleassignment_get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Get privilegedRoleAssignment object. |
|[Delete privilegedRoleAssignment](../api/privilegedroleassignment_delete.md) | None. |Delete privilegedRoleAssignment object. |
|[makePermanent](../api/privilegedroleassignment_makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Make the role assignment as permanent. |
|[makeTemporary](../api/privilegedroleassignment_maketemporary.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Make the role assignment as temporary. |
|[my](../api/privilegedroleassignment_my.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection|Get the requestor's role assignments. |
|[Get privilegedRoleSettings](../api/privilegedrolesettings_get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Retrieve the properties of privilegedRoleSettings object. |
|[Update privilegedRoleSettings](../api/privilegedrolesettings_update.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Update privilegedRoleSettings object. |
|[Get privilegedRoleSummary](../api/privilegedrolesummary_get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Retrieve the privilegedRoleSummary object. |
|[Dismiss privilegedSecurityAlert](../api/privilegedsecurityalert_dismiss.md) |[privilegedSecurityAlert](privilegedsecurityalert.md)| Dismiss a privilegedSecurityAlert.|
|[Fix privilegedSecurityAlert](../api/privilegedsecurityalert_fix.md) |None| Fix a privilegedSecurityAlert.|
|[Get privilegedSecurityAlert](../api/privilegedsecurityalert_get.md) | [privilegedSecurityAlert](privilegedsecurityalert.md) object|Get privilegedSecurityAlert object. |
|[List privilegedSecurityAlert](../api/privilegedsecurityalert_list.md) | [privilegedSecurityAlert](privilegedsecurityalert.md) collection |Get privilegedSecurityAlert object collection. |
|[Reactive privilegedSecurityAlert](../api/privilegedsecurityalert_reactivate.md) |None|Reactive a security alert. |
|[Refresh all privilegedSecurityAlert](../api/privilegedsecurityalert_refreshall.md) |None|Scan the security issues and refresh the security alerts. |
|[Update privilegedSecurityAlert settings](../api/privilegedsecurityalert_update.md) |[privilegedSecurityAlert](../resources/privilegedsecurityalert.md) object|Update the settings for privilegedSecurityAlert object.|
|[canSignUp](../api/privilegedsignupstatus_cansignup.md) |A boolean object in the body.| Check if the requestor is able to sign up the tenant to Privileged Identity Management.|
|[completeSetup](../api/privilegedsignupstatus_completesetup.md) |[roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection object in the response body| Complete the sign up process for the tenant to be managed by Privileged Identity Management.|
|[isSignedUp](../api/privilegedsignupstatus_issignedup.md) |A boolean object in the body.| Check if the tenant has been signed up to Privileged Identity Management.|
|[List privilegedSignupStatus](../api/privilegedsignupstatus_list.md) | [privilegedSignupStatus](privilegedsignupstatus.md) collection |Retrieve the privilegedSignupStatus object for the tenant. |
|[signUp](../api/privilegedsignupstatus_signup.md) | [privilegedSignupStatus](privilegedsignupstatus.md) |Sign up the tenant to Privileged Identity Management.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
