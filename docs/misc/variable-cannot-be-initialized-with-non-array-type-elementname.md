---
title: "无法用非数组类型“&lt;elementname&gt;”初始化变量 | Microsoft Docs"
ms.custom: ""
ms.date: "10/29/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc36536"
  - "bc36536"
helpviewer_keywords: 
  - "BC36536"
ms.assetid: 959415de-164e-4971-aab0-faad315753e9
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 无法用非数组类型“&lt;elementname&gt;”初始化变量
声明为数组的变量必须使用数组值进行初始化。  
  
```  
' Not valid. ' The following line causes this error when executed with Option Strict off. ' Dim arrayVar1() = 10  
```  
  
 **错误 ID：**BC36536  
  
### 更正此错误  
  
-   使用数组值初始化数组变量：  
  
    ```  
    ' With Option Strict off. Dim arrayVar2() = {1, 2, 3} ' With Option Strict on. Dim arrayVar3() As Integer = {1, 2, 3}  
    ```  
  
## 请参阅  
 [NOTINBUILD 一个数组变量](http://msdn.microsoft.com/zh-cn/c2da78bd-6928-46ba-805f-44f819dfaf93)