---
title: "“&lt;method1&gt;”不能重写“&lt;method2&gt;”，因为它是“Declare”语句 | Microsoft Docs"
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
  - "vbc30474"
  - "bc30474"
helpviewer_keywords: 
  - "BC30474"
ms.assetid: 7277e8cc-aa3c-40c3-8682-c8c42d2ee921
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “&lt;method1&gt;”不能重写“&lt;method2&gt;”，因为它是“Declare”语句
你试图重写用 `Declare` 语句声明的基类名称上的委托。  
  
 **错误 ID：**BC30474  
  
### 更正此错误  
  
1.  更改重写的成员，使其不再是 `Declare` 语句。  
  
2.  请勿尝试重写此方法。  
  
## 请参阅  
 [Declare 语句](/dotnet/visual-basic/language-reference/statements/declare-statement)   
 [不在生成中：重写属性和方法](http://msdn.microsoft.com/zh-cn/2167e8f5-1225-4b13-9ebd-02591ba90213)