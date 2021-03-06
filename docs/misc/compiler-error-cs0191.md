---
title: "编译器错误 CS0191 | Microsoft Docs"
ms.custom: ""
ms.date: "11/17/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS0191"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0191"
ms.assetid: 512479e4-656e-4dcb-8d71-801541d72dcd
caps.latest.revision: 10
caps.handback.revision: 10
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0191
无法对属性或索引器“name”赋值 \-\- 它是只读的  
  
 [readonly](/dotnet/csharp/language-reference/keywords/readonly) 字段只能采用构造函数或声明中的一个赋值。 有关详细信息，请参阅[构造函数](/dotnet/csharp/programming-guide/classes-and-structs/constructors)。  
  
 如果 `readonly` 字段为 [static](/dotnet/csharp/language-reference/keywords/static) 并且构造函数没有被标记为 `static`，也会导致 CS0191。  
  
## 示例  
 下面的示例生成 CS0191。  
  
```  
// CS0191.cs class MyClass { public readonly int TestInt = 6;  // OK to assign to readonly field in declaration MyClass() { TestInt = 11; // OK to assign to readonly field in constructor } public void TestReadOnly() { TestInt = 19;                  // CS0191 } public static void Main() { } }  
```