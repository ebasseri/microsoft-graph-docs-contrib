---
title: "teamCreatedEventMessageDetail resource type"
description: "Represents the details of an event message about a created team."
author: "RamjotSingh"
ms.localizationpriority: medium
ms.prod: "microsoft-teams"
doc_type: resourcePageType
---

# teamCreatedEventMessageDetail resource type

Namespace: microsoft.graph

Represents the details of an event message about a created [team](../resources/team.md).
This message is generated when a **team** is created.


Inherits from [eventMessageDetail](../resources/eventmessagedetail.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Initiator of the event.|
|teamDescription|String|Description for the **team**.|
|teamDisplayName|String|Display name of the **team**.|
|teamId|String|Unique identifier of the **team**.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamCreatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## Related content
- [Example response for an event message about a created **team**](/graph/system-messages/#team-created)
- For more information about other types of events, see [System messages](/graph/system-messages).
