---
title: "特性不能应用于 lambda 表达式的参数 | Microsoft Docs"
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
  - "vbc36634"
  - "bc36634"
helpviewer_keywords: 
  - "BC36634"
ms.assetid: ed751d8d-11b7-4210-97e0-0319edff8c34
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 特性不能应用于 lambda 表达式的参数
你已将特性应用到 lambda 表达式定义中的参数，但特性不受支持。 下面的代码会导致此错误。  
  
```vb#  
Sub LambaAttribute()  
    ' Not valid.  
    Dim add1 = _  
    Function(<System.Runtime.InteropServices.InAttribute()> m As Integer) _  
                   m + 1  
End Sub  
```  
  
 **错误 ID：**BC36634  
  
### 更正此错误  
  
-   删除该特性，或请考虑通过将 lambda 表达式更改为正则函数来修订代码。  
  
## 请参阅  
 <xref:System.Runtime.InteropServices.InAttribute>   
 [lambda 表达式](/dotnet/visual-basic/programming-guide/language-features/procedures/lambda-expressions)   
 [不在生成中：Visual Basic 中的特性](http://msdn.microsoft.com/zh-cn/620bfc0e-4582-4c8b-8432-ebc5c3dccc22)