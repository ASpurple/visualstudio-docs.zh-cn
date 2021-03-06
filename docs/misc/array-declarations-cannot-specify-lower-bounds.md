---
title: "数组声明不能指定下限 | Microsoft Docs"
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
  - "vbc30805"
  - "bc30805"
helpviewer_keywords: 
  - "BC30805"
ms.assetid: f2055387-f4dc-4366-89fb-d752929a0258
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 数组声明不能指定下限
数组始终有为零的下限。 可以指定零为下限以使代码更具可读性。 但是，不能指定任何其他下限值。  
  
 **错误 ID：**BC30805  
  
### 更正此错误  
  
-   维度数组作为整体少于元素总数。 例如，`Dim y(6)` 与 `Dim x(3 To 9)` 具有相同的大小（7 个元素）。 你还可以指定 `Dim y(0 To 6)`。  
  
-   使用偏移量模拟非零下限。 下面的示例模拟维度为 3 到 9 的数组。  
  
    ```  
    Const offset As Integer = 3 Dim arrayIndex As Integer ' arrayIndex can vary between 3 and 9. Dim y(0 To 6) ' The preceding statement allocates the same number of elements ' as Dim y(3 To 9). y(arrayIndex - offset) = value ' The preceding statement converts arrayIndex to the ' corresponding index of y.  
    ```  
  
## 请参阅  
 [数组](/dotnet/visual-basic/programming-guide/language-features/arrays/index)   
 [Visual Basic 中的数组维数](/dotnet/visual-basic/programming-guide/language-features/arrays/array-dimensions)   
 [NOTINBUILD 如何：在数组上指定下限为零](http://msdn.microsoft.com/zh-cn/20ffd49a-64f7-4634-8ed0-46ba1049d935)