---
title: "类型“&lt;类型名称1&gt;”的表达式永不属于类型“&lt;类型名称2&gt;” | Microsoft Docs"
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
  - "vbc31430"
  - "bc31430"
helpviewer_keywords: 
  - "BC31430"
ms.assetid: 1d527033-3f6f-4945-b1d3-5ef59a1e1b53
caps.latest.revision: 5
caps.handback.revision: 5
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 类型“&lt;类型名称1&gt;”的表达式永不属于类型“&lt;类型名称2&gt;”
`TypeOf`...`Is` 表达式测试它不能包含的数据类型的对象引用变量。  
  
 在某些情况下，例如，如果两个类之间没有任何继承关系，编译器可以确定 `TypeOf`...`Is` 测试只能失败。  
  
 以下代码会生成此错误。  
  
 `Dim refVar as System.Windows.Forms.Form`  
  
 `If TypeOf refVar Is System.Array`  
  
 `End If`  
  
 因为 <xref:System.Windows.Forms.Form> 和 <xref:System.Array> 是完全不相关的类型，编译器可以确定 `TypeOf`...`Is` 表达式为 `refVar` 的任何值返回 `False`。  
  
 **错误 ID：**BC31430  
  
### 更正此错误  
  
-   测试真实数据类型的变量，或一起删除 `TypeOf`...`Is` 测试。  
  
## 请参阅  
 [TypeOf 运算符](/dotnet/visual-basic/language-reference/operators/typeof-operator)   
 [如何：确定对象变量引用的类型](../Topic/How%20to:%20Determine%20What%20Type%20an%20Object%20Variable%20Refers%20To%20\(Visual%20Basic\).md)