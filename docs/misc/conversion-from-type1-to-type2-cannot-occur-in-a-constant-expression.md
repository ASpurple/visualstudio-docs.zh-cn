---
title: "常量表达式中不会发生从“&lt;type1&gt;”到“&lt;type2&gt;”的转换 | Microsoft Docs"
ms.custom: ""
ms.date: "11/17/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc30060"
  - "vbc30060"
helpviewer_keywords: 
  - "BC30060"
ms.assetid: bea60254-67b6-4881-91d2-47854c4d073c
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 常量表达式中不会发生从“&lt;type1&gt;”到“&lt;type2&gt;”的转换
`Const` 语句的初始化表达式计算出无法转换为所声明的常量类型的数据类型。  
  
 **错误 ID：**BC30060  
  
### 更正此错误  
  
1.  使用可转换为对常量声明的类型的数据类型的表达式初始化常量。  
  
## 请参阅  
 [Const 语句](/dotnet/visual-basic/language-reference/statements/const-statement)   
 [Visual Basic 中的类型转换](/dotnet/visual-basic/programming-guide/language-features/data-types/type-conversions)