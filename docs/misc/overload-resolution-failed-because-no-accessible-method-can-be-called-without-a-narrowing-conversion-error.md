---
title: "重载决策失败，原因是没有可访问的“&lt;method&gt;”能够不经收缩转换即可被调用：&lt;error&gt; | Microsoft Docs"
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
  - "vbc30519"
  - "bc30519"
helpviewer_keywords: 
  - "BC30519"
ms.assetid: 3b3e724d-6fad-4146-b47d-6525493b2fa8
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 重载决策失败，原因是没有可访问的“&lt;method&gt;”能够不经收缩转换即可被调用：&lt;error&gt;
你已调用重载方法，但编译器找不到无需收缩转换便可调用的方法。 收缩转换将值更改为可能无法精确保存某些可能值的数据类型。  
  
 **错误 ID：**BC30519  
  
### 更正此错误  
  
-   指定 `Option Strict Off`。  
  
## 请参阅  
 [重载属性和方法](/dotnet/visual-basic/programming-guide/language-features/objects-and-classes/overloaded-properties-and-methods)   
 [扩大转换和收缩转换](/dotnet/visual-basic/programming-guide/language-features/data-types/widening-and-narrowing-conversions)   
 [Option Strict 语句](/dotnet/visual-basic/language-reference/statements/option-strict-statement)