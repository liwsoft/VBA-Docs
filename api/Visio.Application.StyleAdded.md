---
title: Application.StyleAdded event (Visio)
ms.prod: visio
api_name:
- Visio.Application.StyleAdded
ms.assetid: a966cbc6-529e-5525-5fc2-ed9cd3250dfa
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Application.StyleAdded event (Visio)

Occurs after a new style is added to a document.


## Syntax

_expression_.**StyleAdded** (_Style_)

_expression_ A variable that represents an **[Application](Visio.Application.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Style_|Required| **[IVSTYLE]**|The style that was added to the document.|

## Remarks

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]