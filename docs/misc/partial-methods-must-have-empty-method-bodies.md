---
title: "分部方法的方法体必须为空 | Microsoft Docs"
ms.custom: ""
ms.date: "11/16/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc31435"
  - "vbc31435"
helpviewer_keywords: 
  - "BC31435"
ms.assetid: 279f283d-ce40-401c-8494-4bf06394fdd3
caps.latest.revision: 5
caps.handback.revision: 5
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 分部方法的方法体必须为空
分部方法签名声明的主体不能包含任何代码。 下面的示例演示了分部方法签名及其实现。  
  
```  
' Definition of the partial method signature. Partial Private Sub OnNameChanged() ' The body of the signature is empty. End Sub  
```  
  
```  
' Implementation of the partial method. Private Sub OnNameChanged() MsgBox("Name was changed to " & Me.Name) End Sub  
```  
  
 **错误 ID：**31435  
  
### 更正此错误  
  
-   从分部方法声明中删除任何代码。  
  
## 请参阅  
 [分部方法](/dotnet/visual-basic/programming-guide/language-features/procedures/partial-methods)