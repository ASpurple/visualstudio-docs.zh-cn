---
title: "“Microsoft.VisualBasic.ComClassAttribute”不能应用于被声明为“MustInherit”的类 | Microsoft Docs"
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
  - "BC32508"
  - "vbc32508"
helpviewer_keywords: 
  - "BC32508"
ms.assetid: c8af606d-f448-4703-98df-e594fd511f92
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “Microsoft.VisualBasic.ComClassAttribute”不能应用于被声明为“MustInherit”的类
用 <xref:Microsoft.VisualBasic.ComClassAttribute> 声明类，但其声明指定 `MustInherit`。  
  
 .NET Framework 类必须满足以下要求，才可进行 COM 互操作：  
  
-   它必须为 `Public`，其所有容器必须为 `Public`，且它必须至少公开一个 `Public` 成员。  
  
-   它不能为*抽象*，即它不能用 `MustInherit` 进行声明。  
  
-   它不能为泛型，也不能在泛型容器类型中进行声明。  
  
 **错误 ID:** BC32508  
  
### 更正此错误  
  
-   从类声明中删除 `MustInherit` 关键字。  
  
     \- 或 \-  
  
-   如果类或其包含元素必须为泛型，请从类声明中删除 <xref:Microsoft.VisualBasic.ComClassAttribute>。 不能将其公开给 COM。  
  
## 请参阅  
 <xref:Microsoft.VisualBasic.ComClassAttribute>   
 [COM 互操作](/dotnet/visual-basic/programming-guide/com-interop/index)   
 [MustInherit](/dotnet/visual-basic/language-reference/modifiers/mustinherit)