---
title: "泛型方法中的局部变量不能声明为“Static” | Microsoft Docs"
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
  - "vbc32068"
  - "bc32068"
helpviewer_keywords: 
  - "BC32068"
ms.assetid: cb5df484-76f9-4092-9d19-f26ddcf1c035
caps.latest.revision: 10
caps.handback.revision: 10
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 泛型方法中的局部变量不能声明为“Static”
泛型过程中的局部变量的声明指定 `Static`。  
  
 Visual Basic 和 .NET Framework 当前不支持静态变量与泛型过程的任何组合。  
  
 **错误 ID：**BC32068  
  
### 更正此错误  
  
-   从变量声明中删除 `Static` 关键字。  
  
## 请参阅  
 [Static](/dotnet/visual-basic/language-reference/modifiers/static)   
 [NOTINBUILD 如何：延长变量的生存期](http://msdn.microsoft.com/zh-cn/04e7c56c-1db0-4fe5-a678-859a39ec654b)   
 [Visual Basic 中的泛型类型](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-types)   
 [Visual Basic 中的泛型过程](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-procedures)