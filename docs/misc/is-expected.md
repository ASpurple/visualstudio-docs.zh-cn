---
title: "应为“Is”。 | Microsoft Docs"
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
  - "vbc30224"
  - "bc30224"
helpviewer_keywords: 
  - "BC30224"
ms.assetid: 6b5c34c8-53a8-4b49-b343-19be4d0ebda5
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 应为“Is”。
在没有 `Is` 子句的情况下出现了 `TypeOf` 运算符。  
  
 **错误 ID：**BC30224  
  
### 更正此错误  
  
-   在 `TypeOf` 运算符后面添加 `Is` 子句；例如 `TypeOf MyControl Is ComboBox`。  
  
## 请参阅  
 [比较运算符 \(Visual Basic\)](/dotnet/visual-basic/programming-guide/language-features/operators-and-expressions/comparison-operators)