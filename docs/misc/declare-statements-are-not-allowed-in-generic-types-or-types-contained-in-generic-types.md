---
title: "泛型类型或泛型类型中包含的类型中不允许使用“Declare”语句 | Microsoft Docs"
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
  - "BC32075"
  - "vbc32075"
helpviewer_keywords: 
  - "BC32075"
ms.assetid: c620b67e-70f8-42ac-8292-e9ea484904c3
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 泛型类型或泛型类型中包含的类型中不允许使用“Declare”语句
`Declare` 语句是泛型类或结构的一部分，或某个类或结构在泛型类或结构中声明。  
  
 Visual Basic 和 .NET Framework 当前不支持外部引用和泛型类型的任意组合。 编译器需要外部过程的所有参数和返回类型才能正确调用。  
  
 **错误 ID:** BC32075  
  
### 更正此错误  
  
-   将 `Declare` 语句移到所有泛型类型的作用域之外，或者全部删除。  
  
## 请参阅  
 [Declare 语句](/dotnet/visual-basic/language-reference/statements/declare-statement)   
 [Visual Basic 中的泛型类型](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-types)