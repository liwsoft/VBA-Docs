---
title: Attachment.ColumnWidth property (Access)
keywords: vbaac10.chm14008
f1_keywords:
- vbaac10.chm14008
ms.prod: access
api_name:
- Access.Attachment.ColumnWidth
ms.assetid: 1827efbf-f481-7e26-0638-775a522b2c46
ms.date: 02/07/2019
ms.localizationpriority: medium
---


# Attachment.ColumnWidth property (Access)

Use the **ColumnWidth** property to specify the width of a column in Datasheet view. Read/write **Integer**.


## Syntax

_expression_.**ColumnWidth**

_expression_ A variable that represents an **[Attachment](Access.Attachment.md)** object.


## Remarks

In Visual Basic, the **ColumnWidth** property setting is an **Integer** value that represents the column width in [twips](../language/glossary/vbe-glossary.md#twip). You can specify a width or use one of the following predefined settings.

|Setting|Description|
|:-----|:-----|
|0|Hides the column.|
|1|(Default) Sizes the column to the default width.|

The **ColumnWidth** property applies to all fields in Datasheet view and to form controls when the form is in Datasheet view.

Setting this property to 0, or resizing the field to a zero width in Datasheet view, sets the field's **ColumnHidden** property to **True** (1) and hides the field in Datasheet view.

Setting a field's **ColumnHidden** property to **False** (0) restores the field's **ColumnWidth** property to the value it had before the field was hidden. For example, if the **ColumnWidth** property was 1 prior to the field being hidden by setting the property to 0, changing the field's **ColumnHidden** property to **False** resets the **ColumnWidth** to 1.

The **ColumnWidth** property for a field isn't available when the field's **ColumnHidden** property is set to **True**.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]