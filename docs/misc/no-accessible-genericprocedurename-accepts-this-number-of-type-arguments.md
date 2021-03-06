---
title: "没有可访问的“&lt;genericprocedurename&gt;”接受此数目的类型实参 | Microsoft Docs"
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
  - "bc32118"
  - "vbc32118"
helpviewer_keywords: 
  - "BC32118"
ms.assetid: 4ee942ba-0fa1-4ec1-9c2c-a0c0dc3f1b17
caps.latest.revision: 4
caps.handback.revision: 4
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 没有可访问的“&lt;genericprocedurename&gt;”接受此数目的类型实参
语句调用了具有多个重载版本的泛型过程，但这些重载版本所定义的类型形参数量均不等于调用中所提供的类型实参数量。  
  
 如果只有一个泛型版本，则调用它时不提供类型实参，编译器可以尝试进行*类型推理*。 有关详细信息，请参见 [Visual Basic 中的泛型过程](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-procedures) 中的“类型推理”。 但是，如果存在多个泛型版本，则编译器无法从中进行选择，除非你提供类型实参。 如果提供一个类型实参，则必须为重载版本之一定义的每个类型形参提供一个类型实参。  
  
 **错误 ID：**BC32118  
  
### 更正此错误  
  
-   确定要调用的重载版本，然后将提供相应数量的类型形参。  
  
## 请参阅  
 [Overloads](/dotnet/visual-basic/language-reference/modifiers/overloads)   
 [过程重载](/dotnet/visual-basic/programming-guide/language-features/procedures/procedure-overloading)   
 [Visual Basic 中的泛型类型](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-types)   
 [Visual Basic 中的泛型过程](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-procedures)