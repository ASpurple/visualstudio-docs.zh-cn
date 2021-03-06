---
title: "变量“&lt;variablename&gt;”在赋值前按引用传递 | Microsoft Docs"
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
  - "vbc42030"
  - "BC42030"
helpviewer_keywords: 
  - "BC42030"
ms.assetid: 8f1aae99-f032-4fdf-b6dc-3360cc5b94de
caps.latest.revision: 11
caps.handback.revision: 11
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 变量“&lt;variablename&gt;”在赋值前按引用传递
变量“\<variablename\>”在赋值前按引用传递。 可能在运行时导致 null 引用异常。  
  
 在为变量赋值前，过程调用将变量作为实参传递给 `ByRef` 形参。  
  
 如果从未为变量赋值，则它保持其数据类型的默认值。 对于引用数据类型，默认值是 [Nothing](/dotnet/visual-basic/language-reference/nothing)。 在某些情况下，读取具有 `Nothing` 值的引用变量可能导致 <xref:System.NullReferenceException>。  
  
 将参数传递给过程 `ByRef`，将使该过程能够修改以该参数的基础变量。  
  
 默认情况下，此消息是一个警告。 有关隐藏警告或将警告视为错误的详细信息，请参阅 [在 Visual Basic 中配置警告](../ide/configuring-warnings-in-visual-basic.md)。  
  
 **错误 ID：**BC42030  
  
### 更正此错误  
  
-   如果想让过程通过 `ByRef` 参数为变量赋值而变量是否已持有值并不重要，则无需进行任何操作。  
  
-   如果过程中的逻辑在赋值之前读取参数，且变量是值类型，请确保过程逻辑不取决于变量是否持有其默认值。  
  
-   如果过程中的逻辑在赋值之前读取参数，且变量是值类型，请确保过程逻辑能处理 `Nothing` 值。 例如，可以使用 [Try...Catch...Finally 语句](/dotnet/visual-basic/language-reference/statements/try-catch-finally-statement) 捕获 <xref:System.NullReferenceException>。  
  
## 请参阅  
 [Dim 语句](/dotnet/visual-basic/language-reference/statements/dim-statement)   
 [值类型和引用类型](/dotnet/visual-basic/programming-guide/language-features/data-types/value-types-and-reference-types)   
 [通过值和通过引用传递参数](/dotnet/visual-basic/programming-guide/language-features/procedures/passing-arguments-by-value-and-by-reference)   
 [ByRef](/dotnet/visual-basic/language-reference/modifiers/byref)   
 [变量声明](/dotnet/visual-basic/programming-guide/language-features/variables/variable-declaration)   
 [变量疑难解答](/dotnet/visual-basic/programming-guide/language-features/variables/troubleshooting-variables)