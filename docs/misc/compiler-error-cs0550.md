---
title: "编译器错误 CS0550 | Microsoft Docs"
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
  - "CS0550"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0550"
ms.assetid: 57278c17-443c-40f2-9ebd-853558743564
caps.latest.revision: 9
caps.handback.revision: 9
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器错误 CS0550
“accessor”添加了未在接口成员“property”中找到的访问器  
  
 派生类中属性的实现包含基接口中未指定的访问器。  
  
 有关详细信息，请参阅[使用属性](/dotnet/csharp/programming-guide/classes-and-structs/using-properties)。  
  
## 示例  
 下面的示例生成 CS0550。  
  
```  
// CS0550.cs namespace x { interface ii { int i { get; // add the following accessor to resolve this CS0550 // set; } } public class a : ii { int ii.i { get { return 0; } set {}   // CS0550  no set in interface } public static void Main() {} } }  
```