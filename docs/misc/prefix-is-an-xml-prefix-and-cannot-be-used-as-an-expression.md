---
title: "“prefix”是一个 XML 前缀，不能用作表达式 | Microsoft Docs"
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
  - "bc30114"
  - "vbc30114"
helpviewer_keywords: 
  - "BC30114"
ms.assetid: 5cb7c89e-c61b-483a-9369-5285b7cbcf45
caps.latest.revision: 4
caps.handback.revision: 4
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “prefix”是一个 XML 前缀，不能用作表达式
“prefix”是一个 XML 前缀，不能用作表达式。 使用 GetXmlNamespace 运算符创建命名空间对象。  
  
 使用 `Imports` 语句导入的 XML 命名空间的前缀不能在 XML 文本以外使用。  
  
 **错误 ID：**BC30114  
  
### 更正此错误  
  
-   如果必须引用 XML 命名空间的一部分，请使用 `GetXmlNamespace` 运算符检索 <xref:System.Xml.Linq.XNamespace> 对象。 使用该对象取代 XML 命名空间前缀。  
  
-   如果使用 XML 命名空间前缀来限定 XML 文本，请确保对 XML 文本使用适当的语法。  
  
## 请参阅  
 [XML 文本](/dotnet/visual-basic/language-reference/xml-literals/index)   
 [Imports 语句（XML 命名空间）](/dotnet/visual-basic/language-reference/statements/imports-statement-xml-namespace)   
 [GetXmlNamespace 运算符](/dotnet/visual-basic/language-reference/operators/getxmlnamespace-operator)   
 [XML](/dotnet/visual-basic/programming-guide/language-features/xml/index)   
 [Visual Basic 中的 LINQ 简介](/dotnet/visual-basic/programming-guide/language-features/linq/introduction-to-linq)