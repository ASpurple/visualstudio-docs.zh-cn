---
title: "编译器错误 CS0271 | Microsoft Docs"
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
  - "CS0271"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0271"
ms.assetid: eadc9fb5-7770-4ec4-94f6-3c7cf37eec06
caps.latest.revision: 11
caps.handback.revision: 11
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0271
由于 get 访问器不可访问，因此不能在此上下文中使用属性或索引器“property\/indexer”  
  
 当你尝试访问无法访问的 `get` 访问器时出现此错误。 若要解决此错误，增加访问器的可访问性，或更改调用位置。 有关详细信息，请参阅[访问器可访问性](/dotnet/csharp/programming-guide/classes-and-structs/restricting-accessor-accessibility)和 [属性](/dotnet/csharp/programming-guide/classes-and-structs/properties)。  
  
 以下示例生成 CS0271：  
  
```  
// CS0271.cs public class MyClass { public int Property { private get { return 0; } set { } } public int Property2 { get { return 0; } set { } } } public class Test { public static void Main(string[] args) { MyClass c = new MyClass(); int a = c.Property;   // CS0271 int b = c.Property2;   // OK } }  
```