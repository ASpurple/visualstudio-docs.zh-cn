---
title: "“&lt;typename&gt;”包含声明为“MustOverride”的方法，因此它必须声明为“MustInherit” | Microsoft Docs"
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
  - "vbc31411"
  - "bc31411"
helpviewer_keywords: 
  - "BC31411"
ms.assetid: 5a9f4c57-a4b8-45f5-8273-b7caa689a170
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “&lt;typename&gt;”包含声明为“MustOverride”的方法，因此它必须声明为“MustInherit”
包含 `MustOverride` 成员的类型必须声明为 `MustInherit`。  
  
 **错误 ID：**BC31411  
  
### 更正此错误  
  
-   将 `MustInherit` 修饰符添加到类型。  
  
## 请参阅  
 [MustInherit](/dotnet/visual-basic/language-reference/modifiers/mustinherit)   
 [MustOverride](/dotnet/visual-basic/language-reference/modifiers/mustoverride)