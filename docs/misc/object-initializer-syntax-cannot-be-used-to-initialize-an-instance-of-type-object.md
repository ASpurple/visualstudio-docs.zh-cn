---
title: "对象初始值设定项语法不能用于初始化“Object”的实例 | Microsoft Docs"
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
  - "bc30994"
  - "vbc30994"
helpviewer_keywords: 
  - "BC30994"
ms.assetid: 2ef65965-f014-4fc1-8c7d-c603f0a764df
caps.latest.revision: 5
caps.handback.revision: 5
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 对象初始值设定项语法不能用于初始化“Object”的实例
不可以使用对象初始值设定项语法来初始化 `Object` 的实例。`Object` 的实例没有可供赋值的属性或字段，而对象初始值设定项语法至少需要一个这样的属性或字段。  
  
```  
' Not valid. ' Dim obj1 = New Object With {} ' Dim obj2 = New Object With {.ToString = <some value>}  
```  
  
 **错误 ID：**BC30994  
  
### 更正此错误  
  
1.  声明类型 `Object` 的实例而不使用初始值设定项列表：  
  
    ```  
    Dim obj3 as Object Dim obj4 as New Object()  
    ```  
  
## 请参阅  
 [对象初始值设定项：命名类型和匿名类型](../Topic/Object%20Initializers:%20Named%20and%20Anonymous%20Types%20\(Visual%20Basic\).md)   
 [Object 数据类型](/dotnet/visual-basic/language-reference/data-types/object-data-type)