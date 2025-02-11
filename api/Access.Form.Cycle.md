---
title: Form.Cycle property (Access)
keywords: vbaac10.chm13384
f1_keywords:
- vbaac10.chm13384
ms.prod: access
api_name:
- Access.Form.Cycle
ms.assetid: 621d7101-5237-b239-fcb3-2d942a0329b0
ms.date: 03/12/2019
ms.localizationpriority: medium
---


# Form.Cycle property (Access)

Use the **Cycle** property to specify what happens when you press the Tab key and the focus is in the last control on a bound form. Read/write **Byte**.


## Syntax

_expression_.**Cycle**

_expression_ A variable that represents a **[Form](Access.Form.md)** object.


## Remarks

The **Cycle** property uses the following settings.

|Setting|Visual Basic|Description|
|:-----|:-----|:-----|
|All Records|0|(Default) Pressing the Tab key from the last control on a form moves the focus to the first control in the tab order in the next record.|
|Current Record|1|Pressing the Tab key from the last control on a record moves the focus to the first control in the tab order in the same record.|
|Current Page|2|Pressing the Tab key from the last control on a page moves the focus back to the first control in the tab order on the page.|

You can set the **Cycle** property by using the form's property sheet, a macro, or Visual Basic.

You can set the **Cycle** property in any view.

When you press the Tab key on a form, the focus moves through the controls on the form according to each control's place in the tab order.

You can set the **Cycle** property to All Records for forms designed for data entry. This allows the user to move to a new record by pressing the Tab key.

To move the focus outside a subform control, press Ctrl+Tab.

> [!NOTE] 
> The **Cycle** property only controls the Tab key behavior on the form where the property is set. If a subform control is in the tab order, after the subform control receives the focus, the **Cycle** property setting for the subform determines what happens when you press the Tab key.



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]