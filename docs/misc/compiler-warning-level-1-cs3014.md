---
title: "编译器警告（等级 1）CS3014 | Microsoft Docs"
ms.custom: ""
ms.date: "12/15/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS3014"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS3014"
ms.assetid: 6825b42f-1820-4265-b8d8-9b3387d7c130
caps.latest.revision: 12
caps.handback.revision: 12
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器警告（等级 1）CS3014
由于程序集没有 CLSCompliant 特性，因此“成员”不需要 CLSCompliant 特性  
  
 在没有指定符合公共语言规范 \(CLS\) 的源代码文件中，该文件中的构造将被标记为符合 CLS。 这是不允许的。 若要解决此警告，请将程序集级符合 CLS 的特性添加到文件中（在以下示例中，取消注释包含程序集级特性的行）。 有关 CLS 遵从性的详细信息，请参见[编写符合 CLS 的代码](http://msdn.microsoft.com/zh-cn/4c705105-69a2-4e5e-b24e-0633bc32c7f3)和 [语言独立性和与语言无关的组件](../Topic/Language%20Independence%20and%20Language-Independent%20Components.md)。  
  
## 示例  
 以下示例生成 CS3014:  
  
```  
// CS3014.cs using System; // [assembly:CLSCompliant(true)] public class I { [CLSCompliant(true)]   // CS3014 public void M() { } public static void Main() { } }  
```