---
title: "“Exit AddHandler”、“Exit RemoveHandler”和“Exit RaiseEvent”无效 | Microsoft Docs"
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
  - "vbc31111"
  - "bc31111"
helpviewer_keywords: 
  - "BC31111"
ms.assetid: e02264f3-0645-4de5-b622-8a2a74496b64
caps.latest.revision: 9
caps.handback.revision: 9
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# “Exit AddHandler”、“Exit RemoveHandler”和“Exit RaiseEvent”无效
“Exit AddHandler”、“Exit RemoveHandler”和“Exit RaiseEvent”无效。 使用“Return”退出事件成员。  
  
 `Exit` 语句不能用于退出 `Custom Event` 声明内的 `AddHandler`、`RemoveHandler` 或 `RaiseEvent` 方法。 请改用 `Return` 语句以退出方法，无需指定返回表达式。  
  
 **错误 ID：**BC31111  
  
### 更正此错误  
  
-   用 `Return` 语句替换 `Exit` 语句。  
  
     确保 `Return` 语句不指定返回表达式。  
  
## 请参阅  
 [Event 语句](/dotnet/visual-basic/language-reference/statements/event-statement)   
 [AddHandler \- delete](http://msdn.microsoft.com/zh-cn/fc464cf8-582c-48a6-a9c2-185c4c3d5ff8)   
 [RemoveHandler \- delete](http://msdn.microsoft.com/zh-cn/35c17f61-6e22-4b87-b6e1-3ed0c27a88a0)   
 [RaiseEvent \- delete](http://msdn.microsoft.com/zh-cn/7f765da0-5491-40b6-9ed5-24c98f9daad9)   
 [Return 语句](/dotnet/visual-basic/language-reference/statements/return-statement)   
 [事件](/dotnet/visual-basic/programming-guide/language-features/events/events)