---
title: "无法为 “if” 运算符的第二个和第三个操作数推断出通用类型 | Microsoft Docs"
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
  - "vbc33106"
  - "bc33106"
helpviewer_keywords: 
  - "BC33106"
ms.assetid: 793eed88-a9f9-43e3-b657-c16795ecbbcc
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 无法为 “if” 运算符的第二个和第三个操作数推断出通用类型
无法为 “if” 运算符的第二个和第三个操作数推断出通用类型。 其中一个必须有对另一个的扩大转换。  
  
 当使用三个参数调用 `If` 运算符时，第二个和第三个参数之间必须扩大转换。 例如，由于 `Integer` 和 `String` 之间的两个方向均没有扩大转换，因此以下代码导致此错误。  
  
```vb#  
Dim divisor = 3  
' Not valid.  
' Console.WriteLine(If(divisor <> 0, number \ divisor, "Division by zero"))  
```  
  
 **错误 ID：**BC33106  
  
### 更正此错误  
  
-   如果可能，请在你的代码中为其中一个操作数提供显式转换。  
  
-   使用不同的条件构造，如 `If...Then...Else` 语句。  
  
## 请参阅  
 [If 运算符](/dotnet/visual-basic/language-reference/operators/if-operator)   
 [If...Then...Else 语句](/dotnet/visual-basic/language-reference/statements/if-then-else-statement)   
 [扩大转换和收缩转换](/dotnet/visual-basic/programming-guide/language-features/data-types/widening-and-narrowing-conversions)