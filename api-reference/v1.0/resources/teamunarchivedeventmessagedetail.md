---
title: "teamUnarchivedEventMessageDetail resource type"
description: "Represents the details of an event message about an unarchived team."
author: "RamjotSingh"
ms.localizationpriority: medium
ms.prod: "microsoft-teams"
doc_type: resourcePageType
---

# teamUnarchivedEventMessageDetail resource type

Namespace: microsoft.graph

Represents the details of an event message about an unarchived [team](../resources/team.md).
This message is generated when a **team** is unarchived.


Inherits from [eventMessageDetail](../resources/eventmessagedetail.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Initiator of the event.|
|teamId|String|Unique identifier of the **team**.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamUnarchivedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamUnarchivedEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## Related content
- [Example response for an event message about an unarchived **team**](/graph/system-messages/#team-unarchived)
- For more information about other types of events, see [System messages](/graph/system-messages).
