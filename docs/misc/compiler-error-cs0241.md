---
title: "编译器错误 CS0241 | Microsoft Docs"
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
  - "CS0241"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "默认方法参数值"
  - "默认值，参数值"
  - "默认值，方法参数值"
  - "默认参数值"
  - "CS0241"
ms.assetid: be31b194-3de5-4aab-b23a-6cf790f940ab
caps.latest.revision: 10
caps.handback.revision: 10
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0241
不允许使用默认参数说明符  
  
 [方法参数](/dotnet/csharp/language-reference/keywords/method-parameters)不能有默认值。 如果要达到同样的效果，请使用方法重载。 有关详细信息，请参阅[传递参数](/dotnet/csharp/programming-guide/classes-and-structs/passing-parameters)。  
  
## 示例  
 以下示例生成 CS0241。 此外，该示例演示如何使用重载模拟具有默认参数的方法。  
  
```  
// CS0241.cs public class A { public void Test(int i = 9) {}   // CS0241 } public class B { public void Test() { Test(9); } public void Test(int i)  {} } public class C { public static void Main() { B x = new B(); x.Test(); } }  
```