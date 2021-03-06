---
title: "编译器错误 CS0170 | Microsoft Docs"
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
  - "CS0170"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0170"
ms.assetid: ba881e38-2abf-4a5f-b9e6-28d26a5bd235
caps.latest.revision: 10
caps.handback.revision: 10
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0170
使用了可能未赋值的字段“field”  
  
 结构中的字段在使用前未初始化。 若要解决此问题，首先确定哪个字段尚未初始化，然后将其初始化，再尝试访问该字段。 有关初始化结构的详细信息，请参阅[Struct](/dotnet/csharp/programming-guide/classes-and-structs/structs)和[使用结构](/dotnet/csharp/programming-guide/classes-and-structs/using-structs)。  
  
 下面的示例生成 CS0170：  
  
```  
// CS0170.cs public struct error { public int i; } public class MyClass { public static void Main() { error e; // uncomment the next line to resolve this error // e.i = 0; System.Console.WriteLine( e.i );   // CS0170 because //e.i was never assigned } }  
```