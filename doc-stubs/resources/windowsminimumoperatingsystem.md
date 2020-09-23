---
title: "windowsMinimumOperatingSystem resource type"
description: "The minimum operating system required for a Windows mobile app."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsMinimumOperatingSystem resource type

Namespace: microsoft.graph

The minimum operating system required for a Windows mobile app.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|v10_0|Boolean|Windows version 10.0 or later.|
|v10_1607|Boolean|Windows 10 1607 or later.|
|v10_1703|Boolean|Windows 10 1703 or later.|
|v10_1709|Boolean|Windows 10 1709 or later.|
|v10_1803|Boolean|Windows 10 1803 or later.|
|v10_1809|Boolean|Windows 10 1809 or later.|
|v10_1903|Boolean|Windows 10 1903 or later.|
|v8_0|Boolean|Windows version 8.0 or later.|
|v8_1|Boolean|Windows version 8.1 or later.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": "Boolean",
  "v8_1": "Boolean",
  "v10_0": "Boolean",
  "v10_1607": "Boolean",
  "v10_1703": "Boolean",
  "v10_1709": "Boolean",
  "v10_1803": "Boolean",
  "v10_1809": "Boolean",
  "v10_1903": "Boolean"
}
```
