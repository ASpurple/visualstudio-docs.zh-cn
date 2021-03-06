---
title: "类型约束不能是“NotInheritable”类 | Microsoft Docs"
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
  - "vbc32060"
  - "bc32060"
helpviewer_keywords: 
  - "BC32060"
ms.assetid: f45cc0b6-7df1-462a-b3df-c526c143e16a
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 类型约束不能是“NotInheritable”类
约束列表包括一个标记为[NotInheritable](/dotnet/visual-basic/language-reference/modifiers/notinheritable) 的类。  
  
 类型参数上的约束列表最多能接受一个类。 为该类型形参提供的类型实参必须从该类继承。 因此，类型参数不能接受 *“密封”*或 `NotInheritable`、类作为约束。  
  
 **错误 ID：**BC32060  
  
### 更正此错误  
  
-   如果类型参数必须能够继承自该类，并且你可以控制类的定义，则从类中删除 `NotInheritable` 声明。  
  
-   如果该类必须保持 `NotInheritable`，你不能将其用作约束。 从约束列表中删除类名称。  
  
## 请参阅  
 [Visual Basic 中的泛型类型](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-types)