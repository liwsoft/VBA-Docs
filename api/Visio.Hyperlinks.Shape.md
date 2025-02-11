---
title: Hyperlinks.Shape property (Visio)
keywords: vis_sdr.chm15614320
f1_keywords:
- vis_sdr.chm15614320
ms.prod: visio
api_name:
- Visio.Hyperlinks.Shape
ms.assetid: 4b9d4c86-be67-7b69-ac55-b7e6949ccbe7
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Hyperlinks.Shape property (Visio)

Returns the **Shape** object that owns a **Cell**, **Characters**, **Row**, or **Section** object or that is associated with a **Hyperlink** or **OLEObject** object or with the **Hyperlinks** collection. Read-only.


## Syntax

_expression_.**Shape**

_expression_ A variable that represents a **[Hyperlinks](Visio.Hyperlinks.md)** object.


## Return value

Shape


## Example

This Microsoft Visual Basic for Applications (VBA) macro shows how to use the **Shape** property to get the **Shape** objects that own a **Cell** and a **Characters** object.


```vb
 
Public Sub Shape_Example() 
 
 Dim vsoRectangle As Visio.Shape 
 Dim vsoOval As Visio.Shape 
 Dim vsoShapeFromCell As Visio.Shape 
 Dim vsoShapeFromCharacters As Visio.Shape 
 Dim vsoCell As Visio.Cell 
 Dim vsoCharacters As Visio.Characters 
 
 'Create 2 different shapes and add different text to each shape. 
 Set vsoRectangle = ActivePage.DrawRectangle(2, 3, 5, 4) 
 Set vsoOval = ActivePage.DrawOval(2, 5, 5, 7) 
 vsoRectangle.Text = "Rectangle Shape" 
 vsoOval.Text = "Oval Shape" 
 
 'Get a Cell object from the first shape. 
 Set vsoCell = vsoRectangle.Cells("Width") 
 
 'Get a Characters object from the second shape. 
 Set vsoCharacters = vsoOval.Characters 
 
 'Use the Shape property to get the Shape object. 
 Set vsoShapeFromCell = vsoCell.Shape 
 Set vsoShapeFromCharacters = vsoCharacters.Shape 
 
 'Use each shape's text to verify the proper Shape 
 'object was returned. 
 Debug.Print vsoShapeFromCell.Text 
 Debug.Print vsoShapeFromCharacters.Text 
 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]