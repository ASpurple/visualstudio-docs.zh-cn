---
title: "编译器错误 CS0751 | Microsoft Docs"
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
  - "CS0751"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0751"
ms.assetid: 2ebaed5f-d3ca-452f-8fce-f3299b84360a
caps.latest.revision: 5
caps.handback.revision: 5
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0751
分部方法必须在分部类或分部结构内声明  
  
 除非 [partial](/dotnet/csharp/language-reference/keywords/partial-method) 方法封装在分部类或分部结构内，否则不能对其进行声明。  
  
### 更正此错误  
  
1.  从方法中删除 `partial` 修饰符并提供一个实现，或者将 `partial` 修饰符添加到封闭类或结构。  
  
## 示例  
 下面的示例生成 CS0751：  
  
```  
// cs0751.cs using System; public class C { partial void Part(); // CS0751 public static int Main() { return 1; } }  
```  
  
## 请参阅  
 [分部类和方法](/dotnet/csharp/programming-guide/classes-and-structs/partial-classes-and-methods)