---
title: "“ReadOnly”变量不能作为赋值目标 | Microsoft Docs"
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
  - "vbc30064"
  - "bc30064"
helpviewer_keywords: 
  - "BC30064"
ms.assetid: 17e0751d-4c22-40b2-bb07-cb5c845dbc30
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “ReadOnly”变量不能作为赋值目标
在向其赋值的上下文中找到了 `ReadOnly` 属性。 执行过程中只能向可写的变量、属性和数组元素赋值。  
  
 **错误 ID：**BC30064  
  
### 更正此错误  
  
-   从声明变量的 `Dim` 语句删除 `ReadOnly` 关键字，或者删除对其赋值的语句。  
  
## 请参阅  
 [ReadOnly](/dotnet/visual-basic/language-reference/modifiers/readonly)   
 [Dim 语句](/dotnet/visual-basic/language-reference/statements/dim-statement)