---
title: "mobileAppInstallSummary resource type"
description: "Contains properties for the installation summary of a mobile app."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileAppInstallSummary resource type

Namespace: microsoft.graph

Contains properties for the installation summary of a mobile app.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List installSummary](../api/mobileapp-list-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md) collection|Get the mobileAppInstallSummary resources from the installSummary navigation property.|
|[Create installSummary](../api/mobileapp-post-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Create a new mobileAppInstallSummary object.|
|[Update installSummary](../api/mobileapp-update-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Update the properties of an installSummary object.|
|[Get installSummary](../api/mobileapp-get-mobileappinstallsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Read the properties and relationships of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Delete installSummary](../api/mobileapp-delete-installsummary.md)|None|Delete a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[List mobileAppInstallSummaries](../api/mobileappinstallsummary-list.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md) collection|Get a list of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) objects and their properties.|
|[Create mobileAppInstallSummary](../api/mobileappinstallsummary-create.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Create a new [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Get mobileAppInstallSummary](../api/mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Read the properties and relationships of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Update mobileAppInstallSummary](../api/mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Update the properties of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Delete mobileAppInstallSummary](../api/mobileappinstallsummary-delete.md)|None|Deletes a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Number of Devices that have failed to install this app.|
|failedUserCount|Int32|Number of Users that have 1 or more device that failed to install this app.|
|id|String|Key of the entity.|
|installedDeviceCount|Int32|Number of Devices that have successfully installed this app.|
|installedUserCount|Int32|Number of Users whose devices have all succeeded to install this app.|
|notApplicableDeviceCount|Int32|Number of Devices that are not applicable for this app.|
|notApplicableUserCount|Int32|Number of Users whose devices were all not applicable for this app.|
|notInstalledDeviceCount|Int32|Number of Devices that does not have this app installed.|
|notInstalledUserCount|Int32|Number of Users that have 1 or more devices that did not install this app.|
|pendingInstallDeviceCount|Int32|Number of Devices that have been notified to install this app.|
|pendingInstallUserCount|Int32|Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer",
  "pendingInstallDeviceCount": "Integer",
  "installedUserCount": "Integer",
  "failedUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "notInstalledUserCount": "Integer",
  "pendingInstallUserCount": "Integer"
}
```
