---
title: "编译器错误 CS0133 | Microsoft Docs"
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
  - "CS0133"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0133"
ms.assetid: b5be456f-824d-4e6d-802b-0b1b5889efbd
caps.latest.revision: 8
caps.handback.revision: 8
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0133
指派给“variable”的表达式必须是常量  
  
 [const](/dotnet/csharp/language-reference/keywords/const) 变量不能将非常量表达式作为其值。 有关详细信息，请参阅[常量](/dotnet/csharp/programming-guide/classes-and-structs/constants)。  
  
 下面的示例生成 CS0133：  
  
```  
// CS0133.cs public class MyClass { public const int i = c;   // CS0133, c is not constant public static int c = i; // try the following line instead // public const int i = 6; public static void Main() { } }  
```