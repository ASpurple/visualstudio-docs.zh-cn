---
title: "需要指向程序集“&lt;assemblyname&gt;”（包含事件“&lt;eventname&gt;”的定义）的引用 | Microsoft Docs"
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
  - "vbc30005"
  - "bc30005"
helpviewer_keywords: 
  - "BC30005"
ms.assetid: 843b0b2f-0f93-41c3-8727-13a2138e8140
caps.latest.revision: 10
caps.handback.revision: 10
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 需要指向程序集“&lt;assemblyname&gt;”（包含事件“&lt;eventname&gt;”的定义）的引用
需要指向程序集“\<`assemblyname`\>”（包含事件“\<`eventname`\>”的定义）的引用。 添加对项目的引用。  
  
 事件是在动态链接库 \(DLL\) 或未在项目中直接引用的程序集中定义的。 如果事件是在多个 DLL 或程序集中定义的，则 [!INCLUDE[vbprvb](../code-quality/includes/vbprvb_md.md)] 编译器需要引用以避免多义性。  
  
 **错误 ID：**BC30005  
  
### 更正此错误  
  
-   将未引用的 DLL 或程序集名称包括在项目引用中。  
  
## 请参阅  
 [NIB：引用命名空间和组件](http://msdn.microsoft.com/zh-cn/568fa759-796b-44cd-bf5e-1cf8de6e38fd)   
 [有关无效的引用的疑难解答](../ide/troubleshooting-broken-references.md)