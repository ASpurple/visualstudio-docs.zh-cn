---
title: "编译器警告（等级 3）CS0642 | Microsoft Docs"
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
  - "CS0642"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0642"
ms.assetid: e2df58c0-9b7e-4e50-8e31-e0134955f62c
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器警告（等级 3）CS0642
空语句可能有错误  
  
 conditional 语句后面的分号可能导致代码不按预期执行。  
  
 可以使用 **\/nowarn** 编译器选项或 `#pragmas warning` 禁用此警告；有关详细信息，请参阅 [\/nowarn \(Suppress Specified Warnings\)](/dotnet/csharp/language-reference/compiler-options/nowarn-compiler-option)或 [\#pragma warning](/dotnet/csharp/language-reference/preprocessor-directives/preprocessor-pragma-warning)。  
  
 下面的示例生成 CS0642：  
  
```  
// CS0642.cs // compile with: /W:3 class MyClass { public static void Main() { int i; for (i = 0; i < 10; i += 1);   // CS0642 semicolon intentional? { System.Console.WriteLine (i); } } }  
```