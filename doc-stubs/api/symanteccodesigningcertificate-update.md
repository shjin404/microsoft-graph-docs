---
title: "Update symantecCodeSigningCertificate"
description: "Update the properties of a symantecCodeSigningCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update symantecCodeSigningCertificate
Namespace: microsoft.graph

Update the properties of a [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

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
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object.

The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The key of the entity.|
|content|Binary|The Windows Symantec Code-Signing Certificate in the raw data format.|
|status|certificateStatus|The Cert Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|password|String|The Password required for .pfx file.|
|subjectName|String|The Subject Name for the cert.|
|subject|String|The Subject value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|issuer|String|The Issuer value for the cert.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|uploadDateTime|DateTimeOffset|The Type of the CodeSigning Cert as Symantec Cert.|



## Response

If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/symanteccodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_symanteccodesigningcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-Type: application/json
Content-length: 336

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "content": "Binary",
  "status": "String",
  "password": "String",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "cee297ad-97ad-cee2-ad97-e2cead97e2ce",
  "content": "Binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```
