---
title: "被初始化的字段或属性的名称必须以“.”开头。 | Microsoft Docs"
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
  - "vbc30985"
  - "bc30985"
helpviewer_keywords: 
  - "BC30985"
ms.assetid: 4cb543e1-477c-429c-82df-541ebff08543
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 被初始化的字段或属性的名称必须以“.”开头。
对象初始值设定项列表中的每个成员初始值设定项指定一个字段或属性的名称及其初始值。 字段或属性的名称前必须有一个句点。 例如，对于 `client` 的 `Name` 属性，以下声明将“Microsoft”作为初始值分配。  
  
```  
Dim client As New Customer() With { .Name = "Microsoft" }  
```  
  
 **错误 ID：**BC30985  
  
### 更正此错误  
  
-   使用句点作为每个成员名称的前缀。  
  
## 请参阅  
 [对象初始值设定项：命名类型和匿名类型](../Topic/Object%20Initializers:%20Named%20and%20Anonymous%20Types%20\(Visual%20Basic\).md)   
 [不在生成中：属性过程与字段](http://msdn.microsoft.com/zh-cn/da1c05c1-87c7-40fa-b92c-e9c7e4d170f7)