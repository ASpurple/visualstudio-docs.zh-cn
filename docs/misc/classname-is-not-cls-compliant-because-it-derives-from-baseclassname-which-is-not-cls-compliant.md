---
title: "“&lt;classname&gt;”不符合 CLS，因为它是从不符合 CLS 的“&lt;baseclassname&gt;”派生的 | Microsoft Docs"
ms.custom: ""
ms.date: "12/15/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "vbc40026"
  - "bc40026"
helpviewer_keywords: 
  - "BC40026"
ms.assetid: debcd5e4-75e7-4b14-a6cc-18f1009fe52c
caps.latest.revision: 12
caps.handback.revision: 12
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “&lt;classname&gt;”不符合 CLS，因为它是从不符合 CLS 的“&lt;baseclassname&gt;”派生的
当某一类或接口派生自或实现标记为 `<CLSCompliant(False)>` 的类型时，该类或接口将被标记为 `<CLSCompliant(True)>`。  
  
 为确保类或接口符合 [语言独立性和与语言无关的组件](../Topic/Language%20Independence%20and%20Language-Independent%20Components.md) \(CLS\)，其整个继承层次结构都必须符合。 这意味着从它继承的每一个类型，不管是直接还是间接继承，都必须符合。 同样，如果一个类实现一个或多个接口，则其整个继承层次结构都必须符合。  
  
 当将 <xref:System.CLSCompliantAttribute> 应用到编程元素中时，需要将该特性的 `isCompliant` 参数设置为 `True` 或 `False` 来指示符合或不符合性。 此参数没有默认值，必须为其提供一个值。  
  
 如果不将 <xref:System.CLSCompliantAttribute> 应用到元素，则它将被视为不符合规范。  
  
 默认情况下，此消息是一个警告。 有关隐藏警告或将警告视为错误的信息，请参见 [在 Visual Basic 中配置警告](../ide/configuring-warnings-in-visual-basic.md)。  
  
 **错误 ID：**BC40026  
  
### 更正此错误  
  
-   如果你需要 CLS 符合性，请在不同的继承层次结构或实现方案中定义此类型。  
  
-   如果你要求此类型保留在其当前的继承层次结构或实现方案中，请从其定义中删除 <xref:System.CLSCompliantAttribute>，或将其标记为 `<CLSCompliant(False)>`。  
  
## 请参阅  
 [\<PAVE OVER\>编写符合 CLS 的代码](http://msdn.microsoft.com/zh-cn/4c705105-69a2-4e5e-b24e-0633bc32c7f3)