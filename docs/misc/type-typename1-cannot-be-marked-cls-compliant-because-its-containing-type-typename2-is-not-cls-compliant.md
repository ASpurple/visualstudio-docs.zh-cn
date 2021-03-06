---
title: "类型“&lt;类型名称1&gt;”不能被标记为符合 CLS，因为它的包含类型“&lt;类型名称2&gt;”不符合 CLS | Microsoft Docs"
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
  - "vbc40030"
  - "bc40030"
helpviewer_keywords: 
  - "BC40030"
ms.assetid: f1cfcf04-2a99-46ef-ac87-34cc2099125c
caps.latest.revision: 15
caps.handback.revision: 15
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 类型“&lt;类型名称1&gt;”不能被标记为符合 CLS，因为它的包含类型“&lt;类型名称2&gt;”不符合 CLS
当某一类或接口嵌套于标记为 `<CLSCompliant(False)>` 或未进行标记的类型时，该类或接口将被标记为 `<CLSCompliant(True)>`。  
  
 为确保类或接口符合 [语言独立性和与语言无关的组件](../Topic/Language%20Independence%20and%20Language-Independent%20Components.md) \(CLS\)，整个包含层次结构都必须符合。 这意味着嵌套它的每种类型都必须符合。  
  
 当将 <xref:System.CLSCompliantAttribute> 应用到编程元素中时，需要将该特性的 `isCompliant` 参数设置为 `True` 或 `False` 来指示符合或不符合性。 此参数没有默认值，必须为其提供一个值。  
  
 如果不将 <xref:System.CLSCompliantAttribute> 应用到元素，则它将被视为不符合规范。  
  
 默认情况下，此消息是一个警告。 有关隐藏警告或将警告视为错误的信息，请参见 [在 Visual Basic 中配置警告](../ide/configuring-warnings-in-visual-basic.md)。  
  
 **错误 ID：**BC40030  
  
### 更正此错误  
  
-   如果你需要 CLS 符合性，请在不同的包含层次结构内定义此类型。  
  
-   如果你要求此类型保留在当前的包含层次结构内，请从其定义中删除 <xref:System.CLSCompliantAttribute> 或将其标记为 `<CLSCompliant(False)>`。  
  
## 请参阅  
 [\<PAVE OVER\>编写符合 CLS 的代码](http://msdn.microsoft.com/zh-cn/4c705105-69a2-4e5e-b24e-0633bc32c7f3)