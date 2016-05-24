# privilegedSignupStatus: completeSetup

Complete the sign up process for the organization to be managed by Privileged Identity Management.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Global Administrator_ role. 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedSignupStatus/completeSetup
```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|tenantSetupInfo|tenantSetupInfo|The organization(tenant) setup information that will be used to by the API to do the initial configuration for the organization.|

### Response
If successful, this method returns `200, OK` response code and [roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "privilegedsignupstatus_completesetup"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedSignupStatus/completeSetup
Content-type: application/json
Content-length: 657

{
  "tenantSetupInfo": {
    "id": "id-value",
    "userRolesActions": "userRolesActions-value",
    "firstTimeSetup": true,
    "relevantRolesSettings": [
      "relevantRolesSettings-value"
    ],
    "skipSetup": true,
    "setupStatus": "setupStatus-value",
    "defaultRolesSettings": {
      "minElevationDuration": "datetime-value",
      "maxElavationDuration": "datetime-value",
      "elevationDuration": "datetime-value",
      "id": "id-value",
      "notificationToUserOnElevation": true,
      "ticketingInfoOnElevation": true,
      "mfaOnElevation": true,
      "lastGlobalAdmin": true,
      "isMfaOnElevationConfigurable": true
    }
  }
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleSuccessStatistics",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 213

{
  "value": [
    {
      "roleId": "roleId-value",
      "roleName": "roleName-value",
      "temporarySuccess": 99,
      "temporaryFail": 99,
      "permanentSuccess": 99,
      "permanentFail": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedSignupStatus: completeSetup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
