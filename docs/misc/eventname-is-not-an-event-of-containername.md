---
title: "“&lt;eventname&gt;”不是“&lt;containername&gt;”事件 | Microsoft Docs"
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
  - "vbc30676"
  - "bc30676"
helpviewer_keywords: 
  - "BC30676"
ms.assetid: 16875ec2-94bd-45fd-9198-cc72772d4878
caps.latest.revision: 12
caps.handback.revision: 12
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “&lt;eventname&gt;”不是“&lt;containername&gt;”事件
指定的事件未对此对象声明。  
  
 **错误 ID：**BC30676  
  
### 更正此错误  
  
1.  检查事件的名称的拼写。  
  
2.  检查你是否正在访问正确对象。 使用对对象完全限定的引用，或者使用 `Imports` 语句导入相应的命名空间（如有必要）。  
  
## 请参阅  
 [事件](/dotnet/visual-basic/programming-guide/language-features/events/events)   
 [Imports 语句（.NET 命名空间和类型）](/dotnet/visual-basic/language-reference/statements/imports-statement-net-namespace-and-type)