---
title: "可为 null 的类型的修饰符不能与隐式类型为“Object”的变量一起使用 | Microsoft Docs"
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
  - "bc33112"
  - "vbc33112"
helpviewer_keywords: 
  - "BC33112"
ms.assetid: 50b2a2ad-248d-4faa-820d-bcdf0e8b4aad
caps.latest.revision: 3
caps.handback.revision: 3
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 可为 null 的类型的修饰符不能与隐式类型为“Object”的变量一起使用
变量声明中包括可为 null 的类型修饰符 \(?\)，但未指定一种类型或通过向已声明的变量赋值来推断出某一类型。  
  
 **错误 ID：**BC33112  
  
### 更正此错误  
  
-   声明可为 null 变量时，请指定一种类型。 此类型不能为 <xref:System.Object>。  
  
-   声明可为 null 变量时，请对其进行赋值。 将从所赋的值中推断出可为 null 变量的类型。 值的类型不能为 <xref:System.Object>。  
  
## 请参阅  
 [可以为 Null 的值类型](/dotnet/visual-basic/programming-guide/language-features/data-types/nullable-value-types)