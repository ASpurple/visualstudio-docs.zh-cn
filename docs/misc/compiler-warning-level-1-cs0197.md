---
title: "编译器警告（等级 1）CS0197 | Microsoft Docs"
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
  - "CS0197"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0197"
ms.assetid: 2b5b1b8d-ce13-4bd7-b80a-abb80e9f79ad
caps.latest.revision: 17
caps.handback.revision: 17
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器警告（等级 1）CS0197
由于“argument”是引用封送类的字段，因此，将它作为 ref 或 out 参数传递或获取它的地址可能导致运行时异常  
  
 从 <xref:System.MarshalByRefObject> 直接或间接派生的任何类都是引用封送类。 这样的类可以跨进程和计算机边界引用封送。 因此，此类的实例可以是远程对象的代理。 不能将代理对象的字段作为 [ref](/dotnet/csharp/language-reference/keywords/ref) 或 [out](/dotnet/csharp/language-reference/keywords/out) 传递。 因此，不能传递 `ref` 或 `out` 这类字段，除非实例是 [this](/dotnet/csharp/language-reference/keywords/this)，它不能为代理对象。  
  
## 示例  
 下面的示例生成 CS0197。  
  
```  
// CS0197.cs // compile with: /W:1 class X : System.MarshalByRefObject { public int i; } class M { public int i; static void AddSeventeen(ref int i) { i += 17; } static void Main() { X x = new X(); x.i = 12; AddSeventeen(ref x.i);   // CS0197 // OK M m = new M(); m.i = 12; AddSeventeen(ref m.i); } }  
```