---
title: "“Shared”特性属性“&lt;propertyfield&gt;”不能作为赋值的目标 | Microsoft Docs"
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
  - "bc31500"
  - "vbc31500"
helpviewer_keywords: 
  - "BC31500"
ms.assetid: dffa2b07-9609-4aa3-ae58-c0804d8a05d6
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “Shared”特性属性“&lt;propertyfield&gt;”不能作为赋值的目标
尝试给特性中的 `ReadOnly` 或 `Shared` 属性赋值。  
  
 **错误 ID：**BC31500  
  
### 更正此错误  
  
1.  删除属性赋值语句。  
  
2.  如果使用你开发的属性，请从特性属性中删除 `ReadOnly` 或 `Shared` 修饰符。  
  
## 请参阅  
 [Shared](/dotnet/visual-basic/language-reference/modifiers/shared)   
 [不在生成中：Visual Basic 中的特性](http://msdn.microsoft.com/zh-cn/620bfc0e-4582-4c8b-8432-ebc5c3dccc22)