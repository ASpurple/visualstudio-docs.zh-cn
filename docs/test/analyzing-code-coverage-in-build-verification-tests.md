---
title: "在生成验证测试中分析代码覆盖率 | Microsoft Docs"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: vs-devops-test
ms.tgt_pltfrm: 
ms.topic: article
ms.author: gewarren
manager: ghogen
ms.workload: multiple
author: gewarren
ms.openlocfilehash: 3f02166c89837dfd122ab8a8c71913c659ab1dd2
ms.sourcegitcommit: 7ae502c5767a34dc35e760ff02032f4902c7c02b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2018
---
# <a name="analyzing-code-coverage-in-build-verification-tests"></a>在生成验证测试中分析代码覆盖率
Microsoft Visual Studio 中的代码覆盖率分析显示有多少代码正在被自动测试执行。 有关详细信息，请参阅[使用代码覆盖率确定正在测试的代码数量](../test/using-code-coverage-to-determine-how-much-code-is-being-tested.md)。  
  
 签入代码时，你的测试以及其他团队成员的所有其他测试将在生成服务器中运行。 （如果还没有对此进行设置，请参阅[在生成过程中运行测试](http://msdn.microsoft.com/Library/d05743a1-c5cf-447e-bed9-bed3cb595e38)。）这对于对生成服务分析代码覆盖率很有用，因为这样能提供整个项目中最新和最全面的覆盖率图片。 它还包含用户不常在开发计算机上运行的自动系统测试和其他编码的测试。  
  
1.  在“团队资源管理器”中，打开“生成”，然后添加或编辑生成定义。  
  
2.  在“进程”页中，展开“自动测试”、“测试源”和“运行设置”。 将“运行设置文件的类型”设为“已启用代码覆盖率”。  
  
     如果你有多个测试源定义，请对每个定义重复此步骤。  
  
    -   但是，没有名为“运行设置文件的类型”的字段。  
  
         在“自动测试”下，选择“测试程序集”，然后选择行尾的省略号按钮“[...]”。 在“添加/编辑测试运行”对话框的“测试运行程序”下，选择“Visual Studio 测试运行程序”。  
  
 ![为代码覆盖率设置生成定义](../test/media/codecoverage-plaincc.png "CodeCoverage-plainCC")  
  
 生成运行后，代码覆盖率结果显示在生成摘要中。  
  
## <a name="see-also"></a>请参阅  
 [使用代码覆盖率确定所测试的代码量](../test/using-code-coverage-to-determine-how-much-code-is-being-tested.md)
