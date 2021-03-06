---
title: "转换运算符不能从某一类型转换为相同的类型 | Microsoft Docs"
ms.custom: ""
ms.date: "11/24/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc33024"
  - "vbc33024"
helpviewer_keywords: 
  - "BC33024"
ms.assetid: 4b47bcb0-4f0c-4d1c-9274-cce5b8e2b370
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 转换运算符不能从某一类型转换为相同的类型
用同一类型为参数和返回值声明了转换运算符。  
  
 将任何类型转换为其自身没有意义。  
  
 **错误 ID：**BC33024  
  
### 更正此错误  
  
-   更改参数或返回值的类型。 其中一个必须是此运算符的定义所在的类或结构的类型。 另一个必须是其他类型。  
  
-   如果需要对参数的内容进行转换，请使用 [Function 语句](/dotnet/visual-basic/language-reference/statements/function-statement) 定义 `Function` 过程而不是运算符。  
  
## 请参阅  
 [运算符过程](/dotnet/visual-basic/programming-guide/language-features/procedures/operator-procedures)   
 [Operator 语句](/dotnet/visual-basic/language-reference/statements/operator-statement)   
 [如何：定义运算符](../Topic/How%20to:%20Define%20an%20Operator%20\(Visual%20Basic\).md)   
 [如何：定义转换运算符](../Topic/How%20to:%20Define%20a%20Conversion%20Operator%20\(Visual%20Basic\).md)