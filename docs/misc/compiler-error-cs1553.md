---
title: "编译器错误 CS1553 | Microsoft Docs"
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
  - "CS1553"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS1553"
ms.assetid: aec64251-b4ac-45c0-b143-7ebda138af6e
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS1553
声明无效；请改用“修饰符运算符 \<dest\-type\> \(...”  
  
 [运算符](/dotnet/csharp/language-reference/keywords/operator)的返回类型必须紧跟参数列表，且*修饰符*为 `implicit` 或**隐式**。  
  
 下面的示例生成 CS1553：  
  
```  
// CS1553.cs class MyClass { public static int implicit operator (MyClass f)   // CS1553 // try the following line instead // public static implicit operator int (MyClass f) { return 6; } public static void Main() { } }  
```