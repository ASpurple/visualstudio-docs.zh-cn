---
title: "编译器错误 CS1562 | Microsoft Docs"
ms.custom: ""
ms.date: "11/17/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS1562"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS1562"
ms.assetid: fbadbcc6-9cf2-4af6-b372-fd4e4da4402e
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS1562
必须为没有源的输出指定 \/out 选项  
  
 编译可以创建输出文件，但没有源代码文件可以作为可从中默示输出文件名的输入。 例如，你可能尝试编译仅元数据文件或仅资源文件。  
  
 使用 [\/out](/dotnet/csharp/language-reference/compiler-options/out-compiler-option) 编译器选项指定输出文件的名称。