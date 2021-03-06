---
title: "How to: Extend Code Generated by the O-R Designer | Microsoft Docs"
ms.date: 11/15/2016
ms.prod: visual-studio-dev14
ms.technology: vs-data-tools
ms.topic: conceptual
ms.assetid: d6d1122e-2f55-4607-8d8b-48c3c22600fb
caps.latest.revision: 7
author: jillre
ms.author: jillfra
manager: jillfra
---
# How to: Extend Code Generated by the O/R Designer
[!INCLUDE[vs2017banner](../includes/vs2017banner.md)]

Code generated by the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)] is regenerated when changes are made to the entity classes and other objects on the designer surface. Because of this code regeneration, any code that you add to the generated code is typically overwritten when the designer regenerates code. The [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)] provides the ability to generate partial class files in which you can add code that will not be overwritten. One example of adding your own code to the code generated by the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)] is adding data validation to LINQ to SQL (entity) classes. For information, see [How to: Add validation to entity classes](../data-tools/how-to-add-validation-to-entity-classes.md).

 [!INCLUDE[note_settings_general](../includes/note-settings-general-md.md)]

## Adding Code to an Entity Class

#### To create a partial class and add code to an entity class

1. Open or create a new LINQ to SQL Classes file (**.dbml** file) in the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)]. (Double-click the **.dbml** file in **Solution Explorer**/**Database Explorer**.)

2. In the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)], right-click the class for which you want to add validation and then click **View Code**.

     The Code Editor opens with a partial class for the selected entity class.

3. Add your code in the partial class declaration for the entity class.

## Adding Code to a DataContext

#### To create a partial class and add code to a DataContext

1. Open or create a new LINQ to SQL Classes file (**.dbml** file) in the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)]. (Double-click the **.dbml** file in **Solution Explorer**/**Database Explorer**.)

2. In the [!INCLUDE[vs_ordesigner_short](../includes/vs-ordesigner-short-md.md)], right-click an empty area on the designer and then click **View Code**.

     The Code Editor opens with a partial class for the DataContext.

3. Add your code in the partial class declaration for the DataContext.

## See Also
 [LINQ to SQL Tools in Visual Studio](../data-tools/linq-to-sql-tools-in-visual-studio2.md)
 [Walkthrough: Creating LINQ to SQL Classes (O-R Designer)](https://msdn.microsoft.com/library/35aad4a4-2e8a-46e2-ae09-5fbfd333c233)
 [LINQ to SQL](https://msdn.microsoft.com/library/73d13345-eece-471a-af40-4cc7a2f11655)
 [Walkthrough: Adding Validation to Entity Classes](https://msdn.microsoft.com/library/85b06a02-b2e3-4534-95b8-d077c8d4c1d7)
