---
title: "声明静态变量“&lt;variablename&gt;”时未使用“As”子句；假定为“Object”类型 | Microsoft Docs"
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
  - "vbc42111"
  - "bc42111"
helpviewer_keywords: 
  - "BC42111"
ms.assetid: ca6b625c-21a5-45f7-ac67-282f6993a724
caps.latest.revision: 15
caps.handback.revision: 15
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# 声明静态变量“&lt;variablename&gt;”时未使用“As”子句；假定为“Object”类型
编译器无法推断静态局部变量的数据类型。 在下面的示例中，`Option Strict` 设置为 `Off` 时，`m` 的类型会是 `Object`，无论 `Option Infer` 是设置为 `On` 还是 `Off`。 局部类型推断不适用。  
  
```  
Sub Main() Static m = 10 End Sub  
```  
  
 默认情况下，此消息是一个警告。 有关如何隐藏警告或如何将警告视为错误的信息，请参见 [在 Visual Basic 中配置警告](../ide/configuring-warnings-in-visual-basic.md)。  
  
 **错误 ID：**BC42111  
  
### 解决此警告  
  
-   为静态局部变量指定数据类型。  
  
     例如，如果希望前面示例中的 `m` 具有类型 `Integer`，请在声明中指定该类型。  
  
    ```  
    Sub Main() Static m As Integer = 10 End Sub  
  
    ```  
  
## 请参阅  
 [Dim 语句](/dotnet/visual-basic/language-reference/statements/dim-statement)   
 [NOTINBUILD 如何：延长变量的生存期](http://msdn.microsoft.com/zh-cn/04e7c56c-1db0-4fe5-a678-859a39ec654b)   
 [局部类型推理](/dotnet/visual-basic/programming-guide/language-features/variables/local-type-inference)   
 [Option Infer 语句](/dotnet/visual-basic/language-reference/statements/option-infer-statement)   
 [Static](/dotnet/visual-basic/language-reference/modifiers/static)