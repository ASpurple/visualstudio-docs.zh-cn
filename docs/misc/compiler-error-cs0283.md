---
title: "编译器错误 CS0283 | Microsoft Docs"
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
  - "CS0283"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0283"
ms.assetid: f94a5b84-92c5-4602-894d-6f856d57e0e6
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0283
不能将类型“type”声明为 const  
  
 常数声明中指定的类型必须是 `byte`、`char`、`short`、`int`、`long`、`float`、`double`、`decimal`、`bool`、`string`、枚举类型或赋值为 null 的引用类型。 每个常量表达式必须产生一个目标类型的值，或一个可通过隐式转换转换为目标类型的类型的值。  
  
## 示例  
 以下示例生成 CS0283。  
  
```  
// CS0283.cs struct MyTest { } class MyClass { // To resolve the error but retain the "const-ness", // change const to readonly. const MyTest test = new MyTest();   // CS0283 public static int Main() { return 1; } }  
```