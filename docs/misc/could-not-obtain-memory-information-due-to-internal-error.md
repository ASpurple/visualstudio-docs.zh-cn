---
title: "由于内部错误，无法获取内存信息 | Microsoft Docs"
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
  - "vbrDiagnosticInfo_Memory"
ms.assetid: 1ba8f774-5858-438e-914e-99fddc9e5e7e
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 由于内部错误，无法获取内存信息
对 `My.Computer.Info` 对象的内存信息属性之一的调用失败。  
  
### 更正此错误  
  
-   在对 `My.Computer.Info` 对象的内存信息属性的调用周围添加一个 `Try...Catch` 块。  
  
## 请参阅  
 [My.Computer.Info 对象](/dotnet/visual-basic/language-reference/objects/my-computer-info-object)   
 [Visual Basic 中的异常与错误处理](http://msdn.microsoft.com/zh-cn/3e351e73-cf23-40ab-8b60-05794160529e)   
 [Try...Catch...Finally 语句](/dotnet/visual-basic/language-reference/statements/try-catch-finally-statement)