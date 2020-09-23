---
title: "Create enterpriseCodeSigningCertificate"
description: "Create a new enterpriseCodeSigningCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create enterpriseCodeSigningCertificate
Namespace: microsoft.graph

Create a new [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

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
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The key of the entity.|
|content|Binary|The Windows Enterprise Code-Signing Certificate in the raw data format.|
|status|certificateStatus|The Certificate Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|subjectName|String|The Subject Name for the cert.|
|subject|String|The Subject Value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|issuer|String|The Issuer value for the cert.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|uploadDateTime|DateTimeOffset|The date time of CodeSigning Cert when it is uploaded.|



## Response

If successful, this method returns a `201 Created` response code and an [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_enterprisecodesigningcertificate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-Type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.management.services.api.enterpriseCodeSigningCertificate",
  "content": "Binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.enterpriseCodeSigningCertificate"
}
-->
``` http
HTTP/1.1 201 Created

Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.enterpriseCodeSigningCertificate",
  "id": "bd986eb8-6eb8-bd98-b86e-98bdb86e98bd",
  "content": "Binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```
