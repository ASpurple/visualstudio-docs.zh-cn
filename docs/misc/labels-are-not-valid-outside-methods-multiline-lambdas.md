---
title: "标签在方法/多行 lambda 外无效 | Microsoft Docs"
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
  - "vbc30016"
  - "bc30016"
helpviewer_keywords: 
  - "BC30016"
ms.assetid: 17d12a96-d759-4df9-882c-5e45c1d814a5
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 标签在方法/多行 lambda 外无效
仅可在 `Sub`、`Function`、属性 `Get`、或属性 `Set` 过程中向语句添加标签。 只有可执行语句可以有标签，并且所有可执行语句必须处于过程内。  
  
 **错误 ID：**BC30016  
  
### 更正此错误  
  
1.  从该语句删除的标签或将语句移动到过程内。  
  
## 请参阅  
 [如何：标记语句](../Topic/How%20to:%20Label%20Statements%20\(Visual%20Basic\).md)   
 [Sub 语句](/dotnet/visual-basic/language-reference/statements/sub-statement)   
 [Function 语句](/dotnet/visual-basic/language-reference/statements/function-statement)   
 [Get 语句](/dotnet/visual-basic/language-reference/statements/get-statement)   
 [Set 语句](/dotnet/visual-basic/language-reference/statements/set-statement)