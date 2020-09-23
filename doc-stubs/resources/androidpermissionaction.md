---
title: "androidPermissionAction resource type"
description: "Mapping between an Android app permission and the action Android should take when that permission is requested."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidPermissionAction resource type

Namespace: microsoft.graph

Mapping between an Android app permission and the action Android should take when that permission is requested.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|androidPermissionActionType|Type of Android permission action. Possible values are: `prompt`, `autoGrant`, `autoDeny`.|
|permission|String|Android permission string, defined in the official Android documentation.  Example 'android.permission.READ_CONTACTS'.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```
