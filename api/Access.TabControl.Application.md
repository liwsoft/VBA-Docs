---
title: TabControl.Application property (Access)
keywords: vbaac10.chm12065
f1_keywords:
- vbaac10.chm12065
ms.prod: access
api_name:
- Access.TabControl.Application
ms.assetid: 3074f868-a6e0-954a-3211-251f516f1a6f
ms.date: 03/26/2019
ms.localizationpriority: medium
---


# TabControl.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[TabControl](Access.TabControl.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]