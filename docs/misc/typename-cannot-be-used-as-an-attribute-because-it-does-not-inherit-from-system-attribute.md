---
title: "“&lt;typename&gt;”不从 &quot;System.Attribute&quot; 继承，因此不能用作特性 | Microsoft Docs"
ms.custom: ""
ms.date: "10/29/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc31504"
  - "bc31504"
helpviewer_keywords: 
  - "BC31504"
ms.assetid: 37517623-5099-4db9-a461-f2f5daa4957b
caps.latest.revision: 10
caps.handback.revision: 10
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “&lt;typename&gt;”不从 &quot;System.Attribute&quot; 继承，因此不能用作特性
试图使用并非从 `System.Attribute` 派生的类。  
  
 **错误 ID：**BC31504  
  
### 更正此错误  
  
1.  通过在类代码的第一行添加 `Imports` 语句，将自定义特性定义为从 `System.Attribute` 派生的类。  
  
## 请参阅  
 <xref:System.AttributeUsageAttribute>   
 [不在生成中：Visual Basic 中的自定义特性](http://msdn.microsoft.com/zh-cn/d72d8a5c-8f64-4614-b15b-cad66845d047)