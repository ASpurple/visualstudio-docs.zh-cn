---
title: "“GoTo &lt;labelname&gt;”无效，因为“&lt;labelname&gt;”位于不包含此语句的“Try”，“Catch”或“&#39;Finally”语句内 | Microsoft Docs"
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
  - "bc30754"
  - "vbc30754"
helpviewer_keywords: 
  - "BC30754"
ms.assetid: 2eefc7fb-fdf0-41e9-bf60-c3bc93580e14
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “GoTo &lt;labelname&gt;”无效，因为“&lt;labelname&gt;”位于不包含此语句的“Try”，“Catch”或“&#39;Finally”语句内
你不能分支到 `Try...Catch...Finally` 块。  
  
 **错误 ID：**BC30754  
  
### 更正此错误  
  
-   重构你的代码，以便标签位于 `Try...Catch...Finally` 块之前。  
  
## 请参阅  
 [Try...Catch...Finally 语句](/dotnet/visual-basic/language-reference/statements/try-catch-finally-statement)