---
title: "特性成员“&lt;membername&gt;”不能作为赋值的目标，因为它未声明为“Public” | Microsoft Docs"
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
  - "vbc31511"
  - "bc31511"
helpviewer_keywords: 
  - "BC31511"
ms.assetid: f8c958f6-58a4-4aff-b8c3-f2e9481e8132
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 特性成员“&lt;membername&gt;”不能作为赋值的目标，因为它未声明为“Public”
尝试给特性中的私有成员赋值。  
  
 **错误 ID：**BC31511  
  
### 更正此错误  
  
1.  删除赋值。  
  
2.  如果使用自己开发的自定义特性，将特性成员的访问修饰符更改为 `Public`。  
  
## 请参阅  
 [不在生成中：Visual Basic 中的特性](http://msdn.microsoft.com/zh-cn/620bfc0e-4582-4c8b-8432-ebc5c3dccc22)   
 [Public](/dotnet/visual-basic/language-reference/modifiers/public)