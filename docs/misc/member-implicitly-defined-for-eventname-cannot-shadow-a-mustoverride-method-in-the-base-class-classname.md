---
title: "为“&lt;eventname&gt;”隐式定义的“&lt;member&gt;”不能隐藏基 &lt;class&gt;“&lt;classname&gt;”中的 &quot;MustOverride&quot; 方法 | Microsoft Docs"
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
  - "vbc31413"
  - "bc31413"
helpviewer_keywords: 
  - "BC31413"
ms.assetid: 071706ce-a394-48b6-9afa-751cb50b2576
caps.latest.revision: 11
caps.handback.revision: 11
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 为“&lt;eventname&gt;”隐式定义的“&lt;member&gt;”不能隐藏基 &lt;class&gt;“&lt;classname&gt;”中的 &quot;MustOverride&quot; 方法
指定的事件隐式声明了一个成员，而此成员与使用 `MustOverride` 修饰符声明的方法同名。  
  
 **错误 ID：**BC31413  
  
### 更正此错误  
  
-   从基类的方法中删除 `MustOverride` 修饰符，或为属性或方法提供唯一名称。  
  
## 请参阅  
 [MustOverride](/dotnet/visual-basic/language-reference/modifiers/mustoverride)   
 [事件](/dotnet/visual-basic/programming-guide/language-features/events/events)