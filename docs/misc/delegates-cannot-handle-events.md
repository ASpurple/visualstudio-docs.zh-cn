---
title: "委托无法处理事件 | Microsoft Docs"
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
  - "bc30019"
  - "vbc30019"
helpviewer_keywords: 
  - "BC30019"
ms.assetid: 7f0c7bb9-8e81-44bf-acc5-80d9785708aa
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 委托无法处理事件
委托是一种引用类型，它指向共享过程或对象上的实例过程。 因为它所指向的过程可以通过赋值更改，所以 `Delegate` 语句不能支持 `Handles` 或 `Implements` 子句。  
  
 **错误 ID：**BC30019  
  
### 更正此错误  
  
-   从 `Delegate` 语句中删除 `Handles` 子句。  
  
## 请参阅  
 [不在生成中：委托和 AddressOf 运算符](http://msdn.microsoft.com/zh-cn/7b2ed932-8598-4355-b2f7-5cedb23ee86f)   
 [Delegate 语句](/dotnet/visual-basic/language-reference/statements/delegate-statement)   
 [Handles](/dotnet/visual-basic/language-reference/statements/handles-clause)   
 [Implements 语句](/dotnet/visual-basic/language-reference/statements/implements-statement)