---
title: "编译器错误 CS0215 | Microsoft Docs"
ms.custom: ""
ms.date: "11/17/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS0215"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0215"
ms.assetid: 2060440d-be22-4c10-8b26-43b08b615447
caps.latest.revision: 8
caps.handback.revision: 8
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0215
运算符 True 或 False 的返回类型必须是 bool  
  
 用户定义的 [true](/dotnet/csharp/language-reference/keywords/true) 和 [false](/dotnet/csharp/language-reference/keywords/false) 运算符必须具有 [bool](/dotnet/csharp/language-reference/keywords/bool) 的返回类型。 有关详细信息，请参阅[可重载运算符](/dotnet/csharp/programming-guide/statements-expressions-operators/overloadable-operators)。  
  
 以下示例生成 CS0215：  
  
```  
// CS0215.cs class MyClass { public static int operator true (MyClass MyInt)   // CS0215 // try the following line instead // public static bool operator true (MyClass MyInt) { return true; } public static int operator false (MyClass MyInt)   // CS0215 // try the following line instead // public static bool operator false (MyClass MyInt) { return true; } public static void Main() { } }  
```