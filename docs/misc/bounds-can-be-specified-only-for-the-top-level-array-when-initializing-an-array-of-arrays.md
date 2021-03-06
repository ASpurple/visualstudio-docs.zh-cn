---
title: "初始化数组的数组时，只能指定顶级数组的界限 | Microsoft Docs"
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
  - "bc32014"
  - "vbc32014"
helpviewer_keywords: 
  - "BC32014"
ms.assetid: d8d7155d-82d1-4a25-b9bb-1883e1586383
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 初始化数组的数组时，只能指定顶级数组的界限
交错数组（数组的数组）的数组初始化设置了某个较低级数组的初始长度。 在数组声明语句中只能指定顶级数组的长度。  
  
 **错误 ID：**BC32014  
  
### 更正此错误  
  
1.  删除除顶级数组以外的其他所有数组的长度定义。  
  
2.  在使用 `New` 关键字在后续赋值语句中设置较低级别数组的初始长度。  
  
## 请参阅  
 [NOTINBUILD 一个数组变量](http://msdn.microsoft.com/zh-cn/c2da78bd-6928-46ba-805f-44f819dfaf93)   
 [NOTINBUILD Visual Basic 中的交错数组](http://msdn.microsoft.com/zh-cn/05c12439-ee8f-4fef-ba75-b35402b67ab9)   
 [New 运算符](/dotnet/visual-basic/language-reference/operators/new-operator)