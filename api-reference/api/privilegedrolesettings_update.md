# Update privilegedRoleSettings

Update the properties of privilegedrolesettings object.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Privileged Role Administrator_ role. 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/<id>/settings
```
### Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer <code>|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|elevationDuration|duration|The default role activation duration. The format follows ISO 8601 standard. Example: PT1H.|
|isMfaOnElevationConfigurable|boolean|**true** if the setting of ```mfaOnElevation``` is configurable. **false** otherwise. Note that the service enforces predefined policies to different roles, and the value specified here will be ignored by the service.|
|lastGlobalAdmin|boolean|Internal used only. Always set to **true** here.|
|maxElavationDuration|duration|Maximal duration for a role activation. The format follows ISO 8601 standard. Example: PT1H.|
|mfaOnElevation|boolean|**true** if MFA is required during role activation. **false** otherwise. This value is configurable only if ```isMfaOnElevationConfigurable``` is set as **true** on the service side.|
|minElevationDuration|duration|Minimal duration for a role activation. The format follows ISO 8601 standard. Example: PT1H.|
|notificationToUserOnElevation|boolean|**true** if send notification the user when his role is activated. **false** otherwise.|
|ticketingInfoOnElevation|boolean|**true** if the ticketing information is required when the user activates the role. **false** otherwise.|

### Response
If successful, this method returns a `200 OK` response code and updated [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/<id>/settings
Content-type: application/json
Content-length: 208

{
  "minElevationDuration": "datetime-value",
  "maxElavationDuration": "datetime-value",
  "elevationDuration": "datetime-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "datetime-value",
  "maxElavationDuration": "datetime-value",
  "elevationDuration": "datetime-value",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedrolesettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->