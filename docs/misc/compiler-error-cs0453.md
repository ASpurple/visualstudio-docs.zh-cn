---
title: "编译器错误 CS0453 | Microsoft Docs"
ms.custom: ""
ms.date: "10/29/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS0453"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0453"
ms.assetid: a1bbd09e-6313-4bfd-84bf-bc15a8d214a6
caps.latest.revision: 13
caps.handback.revision: 13
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0453
类型“Type Name”必须是不可以为 null 值的类型，才能将其用作泛型类型或方法“Generic Identifier”中的参数“Parameter Name”  
  
 当你对其上具有 **value** 约束的泛型类型或方法进行实例化时使用一个非值类型的参数，这时会出现此错误。 当你使用可以为 null 的值类型参数时，它也会发生。 请参阅以下示例中的最后两行代码。  
  
## 示例  
 以下代码生成此错误。  
  
```  
// CS0453.cs using System; public class HV<S> where S : struct { } public class H1 : HV<string> { }                   // CS0453 public class H2 : HV<H1> { }                       // CS0453 public class H3<S> : HV<S> where S : class { }     // CS0453 public class H4 : HV<int?> { }                     // CS0453 public class H5 : HV<Nullable<Nullable<int>>> { }  // CS0453  
```