---
title: "“TypeOf ... Is”要求它的左操作数具有引用类型，但此操作数具有类型“&lt;type&gt;” | Microsoft Docs"
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
  - "bc30021"
  - "vbc30021"
helpviewer_keywords: 
  - "BC30021"
ms.assetid: a6e76fc8-9c7f-4e55-8b68-e6e7b03a6737
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “TypeOf ... Is”要求它的左操作数具有引用类型，但此操作数具有类型“&lt;type&gt;”
`TypeOf...Is` 表达式检查对象变量的运行时类型兼容性。 对于值类型未定义此兼容性。  
  
 **错误 ID：**BC30021  
  
### 更正此错误  
  
-   如果 `Option Strict` 为 `Off`，请使用 `TypeName` 或 `VarType` 函数来获取变量的数据类型信息。  
  
-   如果 `Option Strict` 为 `On`，则变量声明决定变量的数据类型。  
  
## 请参阅  
 [比较运算符 \(Visual Basic\)](/dotnet/visual-basic/programming-guide/language-features/operators-and-expressions/comparison-operators)   
 [不在生成中：TypeName 函数 \(Visual Basic\)](http://msdn.microsoft.com/zh-cn/6197bc6c-e8a6-4711-883c-0c95e94e272c)   
 [不在生成中：VarType 函数 \(Visual Basic\)](http://msdn.microsoft.com/zh-cn/e820b6fc-faa6-4de4-836a-0466032dc190)   
 [Option Strict 语句](/dotnet/visual-basic/language-reference/statements/option-strict-statement)