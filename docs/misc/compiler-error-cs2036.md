---
title: "编译器错误 CS2036 | Microsoft Docs"
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
  - "CS2036"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS2036"
ms.assetid: 44b73be4-b792-4735-bdbd-bd757ab22683
caps.latest.revision: 6
caps.handback.revision: 6
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS2036
要使用 \/pdb 选项，必须同时也使用 \/debug 选项。  
  
 仅为调试版本生成程序数据库文件。 因此，**\/pdb** 选项在零售版本中没有意义。  
  
### 更正此错误  
  
-   添加 **\/debug** 编译器选项。  
  
-   删除 **\/pdb** 编译器选项。  
  
## 示例  
 当使用 **\/pdb** 选项但不使用 \/debug 选项对其进行编译时，下面的示例生成 CS2036：  
  
```  
// cs2036.cs // Compile with: /pdb // CS2036 class Test { public static int Main() { return 1; } }  
```  
  
## 请参阅  
 [\/pdb \(Specify Debug Symbol File\)](/dotnet/csharp/language-reference/compiler-options/pdb-compiler-option)   
 [\/debug \(Emit Debugging Information\)](/dotnet/csharp/language-reference/compiler-options/debug-compiler-option)