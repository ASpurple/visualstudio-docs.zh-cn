---
title: "“If”运算符需要两个或三个操作数 | Microsoft Docs"
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
  - "vbc33104"
  - "bc33104"
helpviewer_keywords: 
  - "BC33104"
ms.assetid: 3218f89b-cdcf-4e61-9a40-475a5d7e469d
caps.latest.revision: 6
caps.handback.revision: 6
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “If”运算符需要两个或三个操作数
`If` 运算符仅可接受两个或三个参数。  
  
 **错误 ID：**BC33104  
  
### 更正此错误  
  
-   检查 `If` 表达式，以查看是否可以将运算符数量减少至或扩展到两个或三个参数。  
  
-   请考虑使用另一个条件构造（如 `If...Then...Else` 语句或嵌套的 `If...Then...Else` 语句）来组织这些参数。  
  
## 请参阅  
 [If 运算符](/dotnet/visual-basic/language-reference/operators/if-operator)   
 [If...Then...Else 语句](/dotnet/visual-basic/language-reference/statements/if-then-else-statement)