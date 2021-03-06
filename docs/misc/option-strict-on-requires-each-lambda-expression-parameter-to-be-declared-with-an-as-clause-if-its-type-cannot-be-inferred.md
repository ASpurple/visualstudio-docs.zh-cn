---
title: "Option Strict On 要求使用“As”子句来声明其类型无法推断的每个 lambda 表达式参数 | Microsoft Docs"
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
  - "bc36642"
  - "vbc36642"
helpviewer_keywords: 
  - "BC36642"
ms.assetid: 2aaa62b8-49c9-4ae8-b0f5-08e3f0b5ad10
caps.latest.revision: 6
caps.handback.revision: 6
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# Option Strict On 要求使用“As”子句来声明其类型无法推断的每个 lambda 表达式参数
已经声明了 lambda 表达式中的参数，但未使用 `As` 子句，并且将 `Option Strict` 设置为了“on”。  
  
```  
' Not valid when Option Strict is on. ' Dim increment1 = Function (n) n + 1  
```  
  
 如果可以推断出 `n` 的类型，则上一个声明有效。 例如，如果将上一个 lambda 表达式分配到函数委托 `Del`：  
  
```  
Delegate Function Del(ByVal p As Integer) As Integer  
```  
  
 现在可以从参数 `p` 推断出 `n` 的类型：  
  
```  
Dim increment2 as Del = Function(n) n + 1  
```  
  
 **错误 ID：**BC36642  
  
### 更正此错误  
  
-   将 `As` 子句添加到参数声明：  
  
    ```  
    Dim increment3 = Function (n As Integer) n + 1  
    ```  
  
## 请参阅  
 [lambda 表达式](/dotnet/visual-basic/programming-guide/language-features/procedures/lambda-expressions)