---
title: "不再支持“Line”语句（智能设备/Visual Basic 编译器错误） | Microsoft Docs"
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
  - "vbc30768"
  - "bc30768"
helpviewer_keywords: 
  - "BC30768"
ms.assetid: e7a17c77-06bb-4d33-966e-addb4f51caaf
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 不再支持“Line”语句（智能设备/Visual Basic 编译器错误）
不再支持 `Line` 语句。 文件 I\/O 功能通常可用作 <xref:Microsoft.VisualBasic.FileSystem.LineInput%2A?displayProperty=fullName>，但 .NET Compact Framewor 的目标版本不支持它。  
  
 **错误 ID：**BC30768  
  
### 更正此错误  
  
-   如果执行文件访问，请使用 <xref:System.IO> 命名空间中定义的函数。  
  
-   如果执行图形，则请使用 <xref:System.Drawing.Graphics.DrawLine%2A?displayProperty=fullName>。  
  
## 请参阅  
 <xref:System.IO>   
 <xref:System.Drawing>   
 [使用 Visual Basic 访问文件](/dotnet/visual-basic/developing-apps/programming/drives-directories-files/file-access)