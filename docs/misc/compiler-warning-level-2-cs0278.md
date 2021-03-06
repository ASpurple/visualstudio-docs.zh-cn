---
title: "编译器警告（等级 2）CS0278 | Microsoft Docs"
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
  - "CS0278"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "CS0278"
ms.assetid: 5418cbbe-bcec-4379-a6f6-410987beb96a
caps.latest.revision: 10
caps.handback.revision: 10
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# 编译器警告（等级 2）CS0278
“type”不实现“pattern name”模式。 “method name”具有“method name”歧义。  
  
 C\# 中的多条语句依赖于定义的模式，例如 `foreach` 和 `using`。 例如，`foreach` 依赖于实现“enumerable”模式的集合类。  
  
 如果编译器由于歧义而无法完成匹配，则会出现 CS0278。 例如，“enumerable”模式需要名为 `MoveNext` 的方法，而你的代码可能包含两个名为 `MoveNext` 的方法。 编译器将尝试查找一个要使用的接口，但建议你确定并解决歧义的起因。  
  
 有关详细信息，请参阅[如何：使用 foreach 访问集合类](../Topic/How%20to:%20Access%20a%20Collection%20Class%20with%20foreach%20\(C%23%20Programming%20Guide\).md)。  
  
## 示例  
 下面的示例生成 CS0278：  
  
```  
// CS0278.cs using System.Collections.Generic; public class myTest { public static void TestForeach<W>(W w) where W: IEnumerable<int>, IEnumerable<string> { foreach (int i in w) {}   // CS0278 } }  
```