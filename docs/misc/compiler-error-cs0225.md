---
title: "编译器错误 CS0225 | Microsoft Docs"
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
  - "CS0225"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0225"
ms.assetid: 0b0cd72b-c47a-44d1-9b27-d1a1fad06807
caps.latest.revision: 8
caps.handback.revision: 8
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0225
params 参数必须是一维数组  
  
 当使用 [params](/dotnet/csharp/language-reference/keywords/params) 关键字时，必须指定该数据类型的一维数组。 有关详细信息，请参阅[方法](/dotnet/csharp/programming-guide/classes-and-structs/methods)。  
  
## 示例  
 下面的示例生成 CS0225：  
  
```  
// CS0225.cs public class MyClass { public static void TestParams(params int a)   // CS0225 // try the following line instead // public static void TestParams(params int[] a) { } public static void Main() { TestParams(1); } }  
```