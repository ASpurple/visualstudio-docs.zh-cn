---
title: "访问修饰符“&lt;accessmodifier&gt;”无效 | Microsoft Docs"
ms.custom: ""
ms.date: "11/24/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc31100"
  - "vbc31100"
helpviewer_keywords: 
  - "BC31100"
ms.assetid: 1cd71acc-0b54-4f64-8d61-75b272d293cb
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 访问修饰符“&lt;accessmodifier&gt;”无效
[Get 语句](/dotnet/visual-basic/language-reference/statements/get-statement) 或 [Set 语句](/dotnet/visual-basic/language-reference/statements/set-statement)，用于指定限制性更弱的访问级别，该访问级别的限制性比为包含属性指定的限制性更弱。  
  
 你始终可以为该属性指定访问级别。 此外，还可以至多为其一个属性过程（`Get` 或 `Set`）指定不同的访问级别，条件是该访问级别比属性访问级别限制性更强。 例如，如果该属性是 `Friend`，你可以为属性过程指定 `Private`，但 `Public` 则不可。 无法为两个属性过程指定访问级别。  
  
 **错误 ID：**BC31100  
  
### 更正此错误  
  
-   令属性过程的访问级别的限制性比属性的访问级别更强，或者完全删除访问修饰符。  
  
-   在 [Property 语句](/dotnet/visual-basic/language-reference/statements/property-statement) 中声明限制性较弱的访问级别，并在属性过程之一当中声明限制性更强的访问级别。  
  
## 请参阅  
 [Property 过程](/dotnet/visual-basic/programming-guide/language-features/procedures/property-procedures)   
 [如何：声明具有混合访问级别的属性](../Topic/How%20to:%20Declare%20a%20Property%20with%20Mixed%20Access%20Levels%20\(Visual%20Basic\).md)