---
title: "XML 注释块不能与任何支持应用 XML 文档注释的语言元素相关联 | Microsoft Docs"
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
  - "bc42312"
  - "vbc42312"
helpviewer_keywords: 
  - "BC42312"
ms.assetid: c65b702c-b634-4bfe-82b9-edcac464b494
caps.latest.revision: 14
caps.handback.revision: 14
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# XML 注释块不能与任何支持应用 XML 文档注释的语言元素相关联
XML 注释块不能与任何有效的语言元素相关联。 将忽略该 XML 注释。 如果注释块中的 XML 标记没有任何匹配的语言元素，也会发生此错误。  
  
 **错误 ID:** BC42312  
  
### 更正此错误  
  
-   查找并删除多余的 XML 标记，或者提供其描述的语言元素。  
  
## 请参阅  
 [如何：创建 XML 文档](../Topic/How%20to:%20Create%20XML%20Documentation%20in%20Visual%20Basic.md)   
 [XML 注释标记](/dotnet/visual-basic/language-reference/xmldoc/recommended-xml-tags-for-documentation-comments)