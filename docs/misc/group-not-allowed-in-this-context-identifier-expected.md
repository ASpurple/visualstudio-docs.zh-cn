---
title: "在此上下文中不允许“Group”；应为标识符 | Microsoft Docs"
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
  - "bc36708"
  - "vbc36708"
helpviewer_keywords: 
  - "BC36708"
ms.assetid: ef6b453e-68e7-47c2-997c-9fd1ca074217
caps.latest.revision: 3
caps.handback.revision: 3
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 在此上下文中不允许“Group”；应为标识符
`Group` 关键字包含在 `Aggregate` 子句的 `Into` 部分。`Group` 关键字只在 `Group By` 或 `Group Join` 子句中有效。  
  
 **错误 ID：**BC36618  
  
### 更正此错误  
  
-   将 `Aggregate` 关键字从 `Group` 子句中删除。 你可以将 `Group By` 子句添加到查询以对结果进行分组。  
  
## 请参阅  
 [Aggregate 子句](/dotnet/visual-basic/language-reference/queries/aggregate-clause)   
 [Group By 子句](/dotnet/visual-basic/language-reference/queries/group-by-clause)   
 [Group Join 子句](/dotnet/visual-basic/language-reference/queries/group-join-clause)   
 [Visual Basic 中的 LINQ 简介](/dotnet/visual-basic/programming-guide/language-features/linq/introduction-to-linq)   
 [LINQ](/dotnet/visual-basic/programming-guide/language-features/linq/index)