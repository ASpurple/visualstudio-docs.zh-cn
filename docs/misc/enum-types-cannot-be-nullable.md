---
title: "枚举类型不可以为 null | Microsoft Docs"
ms.custom: ""
ms.date: "11/24/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc32129"
  - "bc32129"
helpviewer_keywords: 
  - "BC32129"
ms.assetid: 9e0fe5c9-72c7-4905-b177-d00cc3469ea9
caps.latest.revision: 6
caps.handback.revision: 6
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 枚举类型不可以为 null
用于声明枚举的基础类型不可以为 null。 例如，下列代码会导致此错误：  
  
```vb#  
'' Not valid. ' Enum exampleEnum As Integer? '     Member declarations. ' End Enum  
```  
  
 **错误 ID：**BC32129  
  
### 更正此错误  
  
-   不在 `Enum` 声明中使用可以为 null 的基础类型。  
  
## 请参阅  
 [可以为 Null 的值类型](/dotnet/visual-basic/programming-guide/language-features/data-types/nullable-value-types)   
 [Enum 语句](/dotnet/visual-basic/language-reference/statements/enum-statement)