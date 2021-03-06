---
title: "非法的调用表达式或索引表达式 | Microsoft Docs"
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
  - "vbc32303"
  - "bc32303"
helpviewer_keywords: 
  - "BC32303"
ms.assetid: eed6a16e-4a44-4f72-b1de-d4212940da37
caps.latest.revision: 10
caps.handback.revision: 10
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 非法的调用表达式或索引表达式
括号中的值遵循不是过程、属性或数组的表达式。  
  
 以下代码会生成此错误。  
  
 `Dim testVariable As Object = Nothing(1)`  
  
 因为 `Nothing` 不采用参数或索引，所以不能将其用于括号。  
  
 **错误 ID：**BC32303  
  
### 更正此错误  
  
-   删除圆括号及其包含的任何值。  
  
## 请参阅  
 [如何：调用返回值的过程](../Topic/How%20to:%20Call%20a%20Procedure%20That%20Returns%20a%20Value%20\(Visual%20Basic\).md)   
 [如何：调用不返回值的过程](../Topic/How%20to:%20Call%20a%20Procedure%20that%20Does%20Not%20Return%20a%20Value%20\(Visual%20Basic\).md)   
 [NOTINBUILD 如何：将值放入数组](http://msdn.microsoft.com/zh-cn/6dddc79c-cf60-41c2-b572-8bfa49b4fe7e)   
 [NOTINBUILD 如何：从数组获得值](http://msdn.microsoft.com/zh-cn/202a6468-8ccb-4864-bd8b-eab3b42d4288)   
 [如何：在属性中放置值](../Topic/How%20to:%20Put%20a%20Value%20in%20a%20Property%20\(Visual%20Basic\).md)   
 [如何：从属性获取值](../Topic/How%20to:%20Get%20a%20Value%20from%20a%20Property%20\(Visual%20Basic\).md)