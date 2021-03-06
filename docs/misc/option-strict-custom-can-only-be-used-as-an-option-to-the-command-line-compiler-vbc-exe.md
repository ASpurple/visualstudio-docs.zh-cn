---
title: "Option Strict Custom 只能用作命令行编译器 (vbc.exe) 的选项 | Microsoft Docs"
ms.custom: ""
ms.date: "11/16/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc31141"
  - "bc31141"
helpviewer_keywords: 
  - "BC31141"
ms.assetid: c32ae8ff-aacc-40b4-960a-6f2d5d246671
caps.latest.revision: 5
caps.handback.revision: 5
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Option Strict Custom 只能用作命令行编译器 (vbc.exe) 的选项
`Option Strict` 语句只采用 `On` 和 `Off` 作为参数；不允许 `Option Strict Custom`。  
  
 使用 `/optionstrict:custom` 编译器选项，当未遵从严格语言语义时发出警告。  
  
 **错误 ID：**BC31141  
  
### 更正此错误  
  
1.  从源代码中删除 `Option Strict Custom`。  
  
2.  指定 `/optionstrict:custom` 选项。 有关更多信息，请参见[\/optionstrict](/dotnet/visual-basic/reference/command-line-compiler/optionstrict)。  
  
## 请参阅  
 [Option \<关键字\> 语句](../Topic/Option%20%3Ckeyword%3E%20Statement.md)   
 [Option Strict 语句](/dotnet/visual-basic/language-reference/statements/option-strict-statement)   
 [\/optionstrict](/dotnet/visual-basic/reference/command-line-compiler/optionstrict)