---
title: "编译器错误 CS1027 | Microsoft Docs"
ms.custom: ""
ms.date: "11/16/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "CS1027"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS1027"
ms.assetid: a6657f0f-5664-47a5-95cf-803f5a0e0c90
caps.latest.revision: 7
caps.handback.revision: 7
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS1027
应输入 \#endif 指令  
  
 未找到与指定 `#if` 指令匹配的`#endif` [预处理器指令](/dotnet/csharp/language-reference/preprocessor-directives/index)。 或者，编译器可能发现了 `#endregion` 指令而 `#if` 块内不存在匹配的 `#region` 指令。  
  
 下面的示例生成 CS1027：  
  
```  
// CS1027.cs #if true   // CS1027, uncomment next line to resolve // #endif namespace x { public class clx { public static void Main() { } } }  
```