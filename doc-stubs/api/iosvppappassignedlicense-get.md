---
title: "Get iosVppAppAssignedLicense"
description: "Read the properties and relationships of an iosVppAppAssignedLicense object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get iosVppAppAssignedLicense
Namespace: microsoft.graph

Read the properties and relationships of an [iosVppAppAssignedLicense](../resources/iosvppappassignedlicense.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /iosVppAppAssignedLicense
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [iosVppAppAssignedLicense](../resources/iosvppappassignedlicense.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_iosvppappassignedlicense"
}
-->
``` http
GET https://graph.microsoft.com/beta/iosVppAppAssignedLicense
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.iosVppAppAssignedLicense"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.management.services.api.iosVppAppAssignedLicense",
    "id": "257d87fe-87fe-257d-fe87-7d25fe877d25",
    "userEmailAddress": "String",
    "userId": "String",
    "userName": "String",
    "userPrincipalName": "String"
  }
}
```
