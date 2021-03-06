---
title: "不能在结构中的 lambda 表达式中使用实例成员和“Me” | Microsoft Docs"
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
  - "vbc36638"
  - "bc36638"
helpviewer_keywords: 
  - "BC36638"
ms.assetid: 5c24a7c7-50f6-4ffb-9ed2-07e2abc4eaf3
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 不能在结构中的 lambda 表达式中使用实例成员和“Me”
从结构中，你已定义了引用结构的实例成员或使用 `Me` 的 lambda 表达式。 以下代码阐释了这两个无效引用。  
  
```vb#  
Structure Structure1 Public InstanceMember As Integer Public Function ExampleFun() As Integer '' The error is caused by use of InstanceMember. 'Dim fun1 = Function() InstanceMember '' The error is caused by use of Me. 'Dim fun2 = Function() Me.InstanceMember 'Return fun1() End Function End Structure  
```  
  
 **错误 ID：**BC36638  
  
### 更正此错误  
  
-   将实例成员分配到局部变量，并在你的语句中使用局部变量。  
  
    ```vb#  
    Public Function ExampleFunFix() As Integer Dim temp = InstanceMember Dim fun1 = Function() temp Return fun1() End Function  
    ```  
  
## 请参阅  
 [lambda 表达式](/dotnet/visual-basic/programming-guide/language-features/procedures/lambda-expressions)   
 [Me](http://msdn.microsoft.com/zh-cn/a65973c7-cf06-4547-9b25-9fba885525c2)   
 [Structure 语句](/dotnet/visual-basic/language-reference/statements/structure-statement)