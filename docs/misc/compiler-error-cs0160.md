---
title: "编译器错误 CS0160 | Microsoft Docs"
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
  - "CS0160"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0160"
ms.assetid: 4ef07061-8ef5-42d9-b043-3f81307d569f
caps.latest.revision: 9
caps.handback.revision: 9
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0160
上一个 catch 子句已经捕获了此类型或超类型（“type”）的所有异常  
  
 一系列 **catch** 语句必须按派生程度降序排列。 例如，派生程度最高的对象必须显示在最前。  
  
 有关详细信息，请参阅[异常处理语句](/dotnet/csharp/language-reference/keywords/exception-handling-statements)和[异常和异常处理](/dotnet/csharp/programming-guide/exceptions/exceptions-and-exception-handling)。  
  
 下面的示例生成 CS0160：  
  
```  
// CS0160.cs public class MyClass2 : System.Exception {} public class MyClass { public static void Main() { try {} catch(System.Exception) {}   // Second-most derived; should be second catch catch(MyClass2) {}   // CS0160  Most derived; should be first catch } }  
```