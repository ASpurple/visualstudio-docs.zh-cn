---
title: "方法“&lt;methodname1&gt;”与分部方法“&lt;methodname2&gt;”的泛型约束不相同。 | Microsoft Docs"
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
  - "bc31438"
  - "vbc31438"
helpviewer_keywords: 
  - "BC31438"
ms.assetid: ea092f0c-661b-49db-80c1-76401fc8bc0b
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 方法“&lt;methodname1&gt;”与分部方法“&lt;methodname2&gt;”的泛型约束不相同。
你已定义某个分部方法实现，此方法实现的泛型约束不同于分部方法声明中的约束。 下面的代码阐释此错误。  
  
```vb#  
Partial Class Class1 Partial Private Sub Test(Of T As Class)(ByVal arg As T) End Sub End Class Partial Class Class1 '' The error occurs here, for Test. 'Private Sub Test(Of T As Structure)(ByVal arg As T) 'End Sub End Class  
```  
  
 **错误 ID：**BC31438  
  
## 请参阅  
 [分部方法](/dotnet/visual-basic/programming-guide/language-features/procedures/partial-methods)   
 [分部](/dotnet/visual-basic/language-reference/modifiers/partial)   
 [Visual Basic 中的泛型过程](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-procedures)