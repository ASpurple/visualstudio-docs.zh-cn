---
title: "编译器错误 CS0238 | Microsoft Docs"
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
  - "CS0238"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0238"
ms.assetid: 9b50c6e2-2c3f-431d-bdb7-557b0ec51626
caps.latest.revision: 8
caps.handback.revision: 8
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0238
因为“member”不是重写，所以无法将其密封  
  
 对还未使用 [override](/dotnet/csharp/language-reference/keywords/override) 进行标记的成员使用了[密封](/dotnet/csharp/language-reference/keywords/sealed)。 有关更多信息，请参见[继承](/dotnet/csharp/programming-guide/classes-and-structs/inheritance)。  
  
 下面的示例生成 CS0238：  
  
```  
// CS0238.cs abstract class MyClass { public abstract void f(); } class MyClass2 : MyClass { public static void Main() { } public sealed void f() // CS0238 // Try the following definition instead: // public override sealed void f() { } }  
```