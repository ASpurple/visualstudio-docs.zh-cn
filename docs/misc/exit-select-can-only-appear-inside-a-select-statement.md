---
title: "&quot;Exit Select&quot; 只能出现在 &quot;Select&quot; 语句内 | Microsoft Docs"
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
  - "vbc30099"
  - "bc30099"
helpviewer_keywords: 
  - "BC30099"
ms.assetid: 37c65fc8-6ad9-456a-80b8-66288c62ef24
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# &quot;Exit Select&quot; 只能出现在 &quot;Select&quot; 语句内
`Exit Select` 语句出现在 `Select` 块之外。`Exit Select` 仅在 `Select` 语句或 `Select Case` 语句和相应 `End Select` 语句之间有效。  
  
 **错误 ID：**BC30099  
  
### 更正此错误  
  
1.  确保 `Exit Select` 之前有一个有效的 `Select` 语句或 `Select Case` 语句，之后有一个有效的 `End Select` 语句。  
  
2.  验证 `Select` 块中的其他控制结构是否被正确终止。  
  
## 请参阅  
 [Select...Case 语句](/dotnet/visual-basic/language-reference/statements/select-case-statement)