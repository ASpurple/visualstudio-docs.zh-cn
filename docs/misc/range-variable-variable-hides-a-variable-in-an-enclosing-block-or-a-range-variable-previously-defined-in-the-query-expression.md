---
title: "范围变量 &lt;variable&gt; 隐藏封闭块中的某个变量或之前在查询表达式中定义的某个范围变量。 | Microsoft Docs"
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
  - "bc30978"
  - "vbc30978"
helpviewer_keywords: 
  - "BC30978"
ms.assetid: 806d94c1-653f-40c0-b1c4-95661c76a392
caps.latest.revision: 4
caps.handback.revision: 4
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 范围变量 &lt;variable&gt; 隐藏封闭块中的某个变量或之前在查询表达式中定义的某个范围变量。
查询中的范围变量的名称与之前在同一范围内定义的某个变量的名称或之前在查询中定义的范围变量的名称相同。  
  
 **错误 ID：**BC30978  
  
### 更正此错误  
  
-   确保查询中的所有范围变量都具有唯一名称，与同一范围内现有的变量名称均不重复。  
  
-   用括号将具有重复控制变量名称的嵌套查询括起来，并隔开每个范围变量的范围。  
  
## 请参阅  
 [Visual Basic 中的 LINQ 简介](/dotnet/visual-basic/programming-guide/language-features/linq/introduction-to-linq)   
 [LINQ](/dotnet/visual-basic/programming-guide/language-features/linq/index)