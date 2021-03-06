---
title: "通过使用修改独立的 Shell。Vsct 文件 |Microsoft 文档"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: vs-ide-sdk
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords: Visual Studio shell, isolated mode, .vsct file
ms.assetid: 6d147c2d-10e9-400e-b8ce-5566287b41ba
caps.latest.revision: "8"
author: gregvanl
ms.author: gregvanl
manager: ghogen
ms.workload: vssdk
ms.openlocfilehash: 631aaaf4bf3d36cf5b83c8e67791c453cdfed925
ms.sourcegitcommit: 32f1a690fc445f9586d53698fc82c7debd784eeb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="modifying-the-isolated-shell-by-using-the-vsct-file"></a>通过使用修改独立的 Shell。Vsct 文件
Visual Studio 独立的 shell 项目的 UI 项目包含一个允许你指定哪些应用程序组和单个命令可以在应用程序的.vsct 文件。 以下是一个未修改的.vsct 文件的摘录。  
  
```  
<!-- <Define name="No_WindowListCommand"/> -->  
<!-- <Define name="No_MoreWindowsCommand"/> -->  
<!-- <Define name="No_PaneNextPaneCommand"/> -->  
<!-- <Define name="No_PanePrevPaneCommand"/> -->  
```  
  
 默认情况下，大多数命令和命令组会包括。 若要排除的命令或命令组，只需取消注释该命令或组。  
  
 例如，若要删除的下一个窗格和上一个窗格命令，取消注释`No_PaneNextPaneCommand`和`No_PanePrevPaneCommand`条目：  
  
```  
  
<Define name="No_PaneNextPaneCommand"/> <Define name="No_PanePrevPaneCommand"/>  
  
```  
  
 有关更详细示例这些自定义项，请参阅[演练： 创建基本的独立 Shell 应用程序](walkthrough-creating-a-basic-isolated-shell-application.md)。  
  
## <a name="referenced-files"></a>引用的文件  
 为应用程序的默认.vsct 文件引用以下文件。 这些文件位于 Visual Studio SDK 安装目录的 \VisualStudioIntegration\Common\Inc\ 子目录中。  
  
|文件|描述|  
|----------|-----------------|  
|wbids.h|Web 浏览包的用户界面标识。|  
|AppIDCmdUsed.vsct|主要的 Visual Studio UI 元素的命令表。|  
|EmulatorCmdUsed.vsct|Emacs 和简述编辑器仿真 UI 元素的命令表。|  
|Vsdebugguids.h|定义的命令、 选项页上和其他功能的 Visual Studio 调试器的 Guid。|  
|VsDbgCmdUsed.vsct|调试器的命令表。|  
  
 AppIDCmdUsed.vsct 文件包括基于应用程序.vsct 文件中定义的符号的 Visual Studio UI 元素。  
  
 有关详细信息，请参阅[设计 XML 命令表 (。Vsct) 文件](../internals/designing-xml-command-table-dot-vsct-files.md)和[VSCT XML 架构参考](../vsct-xml-schema-reference.md)。  
  
## <a name="see-also"></a>请参阅  
 [Visual Studio 独立 Shell](visual-studio-isolated-shell.md)