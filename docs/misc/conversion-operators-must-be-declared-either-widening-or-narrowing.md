---
title: "转换运算符必须声明为“Widening”或者“Narrowing”。 | Microsoft Docs"
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
  - "vbc33017"
  - "bc33017"
helpviewer_keywords: 
  - "BC33017"
ms.assetid: 5972d955-ce1d-4348-a021-167eecb3a507
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 转换运算符必须声明为“Widening”或者“Narrowing”。
[Operator 语句](/dotnet/visual-basic/language-reference/statements/operator-statement) 未指定 [Widening](/dotnet/visual-basic/language-reference/modifiers/widening) 或 [Narrowing](/dotnet/visual-basic/language-reference/modifiers/narrowing)。  
  
 在定义转换运算符时，必须将其声明为 `Widening` 或 `Narrowing`。 由于这些特征相互排斥，因此你不能同时指定两者。  
  
 **错误 ID：**BC33017  
  
### 更正此错误  
  
-   决定转换运算符将为 `Widening` 还是 `Narrowing`，并在 `Operator` 语句中包括适当的关键字。 你必须指定一个或另一个。  
  
## 请参阅  
 [扩大转换和收缩转换](/dotnet/visual-basic/programming-guide/language-features/data-types/widening-and-narrowing-conversions)   
 [运算符过程](/dotnet/visual-basic/programming-guide/language-features/procedures/operator-procedures)   
 [Operator 语句](/dotnet/visual-basic/language-reference/statements/operator-statement)   
 [如何：定义运算符](../Topic/How%20to:%20Define%20an%20Operator%20\(Visual%20Basic\).md)   
 [如何：定义转换运算符](../Topic/How%20to:%20Define%20a%20Conversion%20Operator%20\(Visual%20Basic\).md)