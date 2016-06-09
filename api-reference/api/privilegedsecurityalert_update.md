# Update privilegedSecurityAlert settings

Update the settings for privilegedSecurityAlert object.
### Prerequisites
The following **scopes** are required to execute this API: _Directory.AccessAsUser.All_

The requestor needs to have _Privileged Role Administrator_ role.
 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedSecurityAlerts/<id>
```
### Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer <code>|

### Request body
In the request body, supply the values for relevant alert settings that should be updated.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|NumberOfDaysForInactiveAssignment|string|Number of days without role activation. For alert "Redundant administrators increase your attack surface" only.|
|ThresholdGlobalAdminRole|string|Minimum number of Global Administrators to trigger computation of percentage. For alert "Too many global administrators increases your attack surface" only.|
|ThresholdPercentageOfGlobalAdminsOutOfAdmins|string|Percentage of Global Administrators to trigger an alert. For alert "Too many global administrators increases your attack surface" only.|
|TimeIntervalBetweenActivationsInMin|string|Activation renewal time frame in minutes. For alert "Suspicious activation renewals of privileged roles" only.|
|SequentialActivationCounterThreshold|string|Number of renewals within the time frame window to trigger an alert. For alert "Suspicious activation renewals of privileged roles" only.|

### Response
If successful, this method returns a `200 OK` response code and updated [privilegedSecurityAlert](../resources/privilegedsecurityalert.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedsecurityalert"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedSecurityAlerts/<id>
Content-type: application/json
Content-length: 203

{"id":"da5d0491-89e-4f06-893a-81e8171e647d",
"TimeIntervalBetweenActivationsInMin":"310",
"SequentialActivationCounterThreshold":"10"}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedSecurityAlert"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedsecurityalert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
