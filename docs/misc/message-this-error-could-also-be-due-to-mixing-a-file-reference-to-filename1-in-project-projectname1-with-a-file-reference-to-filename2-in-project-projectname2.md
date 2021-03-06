---
title: "&lt;message&gt; 此错误也可能是由于混合了项目“&lt;projectname1&gt;”中“&lt;filename1&gt;”的文件引用和项目“&lt;projectname2&gt;”中“&lt;filename2&gt;”的文件引用所引起 | Microsoft Docs"
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
  - "bc30970"
  - "vbc30970"
helpviewer_keywords: 
  - "BC30970"
ms.assetid: 81cc4f7b-cc16-46cc-9a49-74980300e158
caps.latest.revision: 8
caps.handback.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# &lt;message&gt; 此错误也可能是由于混合了项目“&lt;projectname1&gt;”中“&lt;filename1&gt;”的文件引用和项目“&lt;projectname2&gt;”中“&lt;filename2&gt;”的文件引用所引起
\<message\> 此错误也可能是由于混合了项目“\<projectname1\>”中“\<filepathname1\>”的文件引用和项目“\<projectname2\>”中“\<filepathname2\>”的文件引用所引起。  如果两个程序集完全相同，请尝试更换这些引用，以确保两个引用都来自相同的位置。  
  
 你项目中的代码访问了另一个项目的成员，但你的解决方案配置不允许使用 [!INCLUDE[vbprvb](../code-quality/includes/vbprvb_md.md)] 编译器来解析引用。  
  
 若要访问另一个程序集中定义的类型，[!INCLUDE[vbprvb](../code-quality/includes/vbprvb_md.md)] 编译器必须具有对该程序集的引用。 此引用必须单一、明确，不会导致项目之间循环引用。  
  
 **错误 ID：**BC30970  
  
### 更正此错误  
  
1.  确定产生最佳程序集引用的项目。 为便于确定，你可以使用文件访问轻松程度和更新频率等条件。  
  
2.  在项目属性中，添加对包含某程序集的文件的引用，该程序集定义正在使用的类型。  
  
## 请参阅  
 [管理项目中的引用](../ide/managing-references-in-a-project.md)   
 [NIB：引用命名空间和组件](http://msdn.microsoft.com/zh-cn/568fa759-796b-44cd-bf5e-1cf8de6e38fd)   
 [NOTINBUILD：当多个变量具有相同名称时解析引用](http://msdn.microsoft.com/zh-cn/9601e39f-1911-44e1-ace5-3f6e090408b9)   
 [NIB 如何：使用“添加引用”对话框添加或删除引用](http://msdn.microsoft.com/zh-cn/3bd75d61-f00c-47c0-86a2-dd1f20e231c9)   
 [NIB 如何：修改项目属性和配置设置](http://msdn.microsoft.com/zh-cn/e7184bc5-2f2b-4b4f-aa9a-3ecfcbc48b67)   
 [有关无效的引用的疑难解答](../ide/troubleshooting-broken-references.md)