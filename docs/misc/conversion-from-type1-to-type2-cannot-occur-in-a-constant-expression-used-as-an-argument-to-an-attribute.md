---
title: "在用作特性参数的常量表达式中不能发生从“&lt;type1&gt;”到“&lt;type2&gt;”的转换 | Microsoft Docs"
ms.custom: ""
ms.date: "12/15/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc30934"
  - "vbc30934"
helpviewer_keywords: 
  - "BC30934"
ms.assetid: 120e05f9-1d0e-4800-b05c-a8373e286b9b
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 在用作特性参数的常量表达式中不能发生从“&lt;type1&gt;”到“&lt;type2&gt;”的转换
特性参数所用的表达式计算出不同于对应特性参数的数据类型，且 [!INCLUDE[vbprvb](../code-quality/includes/vbprvb_md.md)] 不允许对特性参数进行所需的类型转换。  
  
 特性为其应用到的元素提供元数据，且编译器必须能够在编译时构造所有元数据。 因此，每个特性必须使用在编译时是常量的值，所以，每个特性参数必须计算出编译时常量值。  
  
 某些类型转换无法生成在编译时是常量的值。 例如，将 `String` 转换为 `Double` 或 `Date` 取决于运行时的区域设置。 其他转换（如派生类型数组转换为 `Object` 数组）则存在各种不允许编译器在特性参数上允许这些转换的问题。  
  
 **错误 ID：**BC30934  
  
### 更正此错误  
  
-   使用计算出与对应参数（由特性定义）具有相同数据类型的表达式。  
  
## 请参阅  
 [不在生成中：Visual Basic 中的特性](http://msdn.microsoft.com/zh-cn/620bfc0e-4582-4c8b-8432-ebc5c3dccc22)   
 [不在生成中：特性的应用程序](http://msdn.microsoft.com/zh-cn/2b1703ed-4437-49b3-bc0b-568094324f47)   
 [Const 语句](/dotnet/visual-basic/language-reference/statements/const-statement)   
 [Visual Basic 中的类型转换](/dotnet/visual-basic/programming-guide/language-features/data-types/type-conversions)