---
title: "需要的对模块“&lt;模块名称&gt;”（包含基类“&lt;类名称&gt;”）的引用 | Microsoft Docs"
ms.custom: ""
ms.date: "12/15/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc30008"
  - "bc30008"
helpviewer_keywords: 
  - "BC30008"
ms.assetid: ec8de475-8a8b-4aa5-86c9-6fcc44dcec06
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 需要的对模块“&lt;模块名称&gt;”（包含基类“&lt;类名称&gt;”）的引用
需要的对模块“\<模块名称\>”（包含基类“\<类名称\>”）的引用。 请向项目中添加一个。  
  
 类在项目不直接引用的模块中定义。 如果类在多个模块中定义，则 [!INCLUDE[vbprvb](../code-quality/includes/vbprvb_md.md)] 编译器需要一个引用以避免多义性。  
  
 **错误 ID：**BC30008  
  
### 更正此错误  
  
-   将未引用模块的名称包括在项目引用中。  
  
## 请参阅  
 [NIB：引用命名空间和组件](http://msdn.microsoft.com/zh-cn/568fa759-796b-44cd-bf5e-1cf8de6e38fd)   
 [有关无效的引用的疑难解答](../ide/troubleshooting-broken-references.md)