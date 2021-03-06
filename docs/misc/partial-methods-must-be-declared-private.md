---
title: "分部方法必须声明为“Private” | Microsoft Docs"
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
  - "vbc31432"
  - "bc31432"
helpviewer_keywords: 
  - "BC31432"
ms.assetid: 3a4474d9-661e-4793-9624-30cf81faddcf
caps.latest.revision: 7
caps.handback.revision: 7
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 分部方法必须声明为“Private”
在分部方法声明中需要具有访问修饰符 `Private`。 下面的示例演示如何在方法签名及其实现中使用 `Private`。  
  
```vb#  
' Definition of the partial method signature. Partial Private Sub OnNameChanged() ' The body of the signature is empty. End Sub  
```  
  
```vb#  
' Implementation of the partial method. Private Sub OnNameChanged() MsgBox("Name was changed to " & Me.Name) End Sub  
```  
  
 **错误 ID：**BC31432  
  
### 更正此错误  
  
-   在签名和实现声明中，将关键字 `Private` 添加到 `Sub` 之前。  
  
## 请参阅  
 [分部方法](/dotnet/visual-basic/programming-guide/language-features/procedures/partial-methods)