---
title: "编译器警告（等级 4）CS0628 | Microsoft Docs"
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
  - "CS0628"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0628"
ms.assetid: a54cfad8-27c9-4abb-8c83-982615489a10
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器警告（等级 4）CS0628
“member”：在密封类中声明了新的保护成员  
  
 [密封](/dotnet/csharp/language-reference/keywords/sealed)类不能引入[保护](/dotnet/csharp/language-reference/keywords/protected)成员，因为其他类不能继承 `sealed` 类并使用 `protected` 成员。  
  
 下面的示例生成 CS0628：  
  
```  
// CS0628.cs // compile with: /W:4 sealed class C { protected int i;   // CS0628 } class MyClass { public static void Main() { } }  
```