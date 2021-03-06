---
title: "编译器错误 CS0274 | Microsoft Docs"
ms.custom: ""
ms.date: "11/16/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS0274"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0274"
ms.assetid: bbd2d64e-a756-4713-b9ed-711d50b65e00
caps.latest.revision: 10
caps.handback.revision: 10
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0274
不能为属性或索引器“property\/indexer”的两个访问器同时指定可访问性修饰符  
  
 当你声明一个在两个访问器上都有访问修饰符的属性或索引器时，将出现此错误。 若要解决此错误，请仅在两个访问器的其中一个上使用访问修饰符。 有关详细信息，请参阅[访问器可访问性](/dotnet/csharp/programming-guide/classes-and-structs/restricting-accessor-accessibility)。  
  
 下面的示例生成 CS0274：  
  
```  
// CS0274.cs public class MyClass { public int Property   // CS0274 { public get { return 0; } protected set { } } }  
```