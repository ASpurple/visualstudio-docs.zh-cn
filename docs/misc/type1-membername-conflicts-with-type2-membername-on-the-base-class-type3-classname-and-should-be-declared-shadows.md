---
title: "&lt;type1&gt;“&lt;membername&gt;”与基类 &lt;type3&gt;“&lt;classname&gt;”上的 &lt;type2&gt;“&lt;membername&gt;”冲突，且应声明为“Shadows” | Microsoft Docs"
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
  - "bc40004"
  - "vbc40004"
helpviewer_keywords: 
  - "BC40004"
ms.assetid: 24d10f31-3b3d-448c-b928-fc937e1f4a92
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# &lt;type1&gt;“&lt;membername&gt;”与基类 &lt;type3&gt;“&lt;classname&gt;”上的 &lt;type2&gt;“&lt;membername&gt;”冲突，且应声明为“Shadows”
以基类中定义的元素的相同名称来声明编程元素。 在这种情况下，此类中的元素应隐藏基类元素。  
  
 此消息是一个警告。 默认假定 `Shadows`。 有关隐藏警告或将警告视为错误的详细信息，请参阅[在 Visual Basic 中配置警告](../ide/configuring-warnings-in-visual-basic.md)。  
  
 **错误 ID：**BC40004  
  
### 更正此错误  
  
-   将 `Shadows` 关键字添加到声明中，或更改所声明的元素的名称。  
  
## 请参阅  
 [Shadows](/dotnet/visual-basic/language-reference/modifiers/shadows)   
 [Visual Basic 中的隐藏](/dotnet/visual-basic/programming-guide/language-features/declared-elements/shadowing)