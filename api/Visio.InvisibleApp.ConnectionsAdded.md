---
title: InvisibleApp.ConnectionsAdded event (Visio)
ms.prod: visio
api_name:
- Visio.InvisibleApp.ConnectionsAdded
ms.assetid: 635d640f-305b-4d9c-10c2-750f7f29cc00
ms.date: 06/25/2019
ms.localizationpriority: medium
---


# InvisibleApp.ConnectionsAdded event (Visio)

Occurs after connections have been established between shapes.


## Syntax

_expression_.**ConnectionsAdded** (_Connects_)

_expression_ A variable that represents an **[InvisibleApp](Visio.InvisibleApp.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Connects_|Required| **[IVCONNECTS]**|The connections that were established.|

## Remarks

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).

> [!NOTE] 
> Use VBA **WithEvents** variables to sink the **ConnectionsDeleted** event.

For performance considerations, the **Document** object's event set does not include the **ConnectionsAdded** event. To sink the **ConnectionsAdded** event from a **Document** object (and the **[ThisDocument](../visio/Concepts/about-the-thisdocument-object-visio.md)** object in a VBA project), you must use the **AddAdvise** method.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]