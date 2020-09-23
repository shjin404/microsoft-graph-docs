---
title: "iosStoreApp: getRelatedAppStates"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# iosStoreApp: getRelatedAppStates
Namespace: microsoft.graph

**TODO: Add Description**

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
GET ** Entity URI for microsoft.management.services.api.iosStoreApp not found/getRelatedAppStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|userPrincipalName|String|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|



## Response

If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/mobileapprelationshipstate.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "iosstoreapp_getrelatedappstates"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.management.services.api.iosStoreApp not found/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.mobileAppRelationshipState)"
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState"
    }
  ]
}
```
