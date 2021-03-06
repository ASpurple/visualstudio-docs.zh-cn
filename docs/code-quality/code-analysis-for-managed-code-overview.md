---
title: "代码分析为托管的代码概述 |Microsoft 文档"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: vs-ide-code-analysis
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: vs.projectpropertypages.codeanalysis
helpviewer_keywords:
- code analysis, managed code
- managed code, code analysis
author: gewarren
ms.author: gewarren
manager: ghogen
ms.workload: dotnet
ms.openlocfilehash: b705abb680276faf9d4311cd21cae1b103c4a09d
ms.sourcegitcommit: 32f1a690fc445f9586d53698fc82c7debd784eeb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="code-analysis-for-managed-code-overview"></a>代码分析托管的代码概述

针对托管代码的代码分析用于分析托管程序集并报告有关程序集的信息，例如 Microsoft .NET Framework 设计准则中规定的编程和设计规则的冲突。

分析工具将它在分析期间执行的检查表示为警告消息。 警告消息标识任何相关的编程和设计问题，如有可能，还提供有关如何修复问题的信息。

## <a name="ide-integrated-development-environment-integration"></a>IDE （集成的开发环境） 集成

手动或自动，可以对你的项目中运行代码分析。

若要生成项目每次运行代码分析，选择**生成时启用代码分析**项目的属性页上。 有关详细信息，请参阅[如何： 启用和禁用自动代码分析](../code-quality/how-to-enable-and-disable-automatic-code-analysis-for-managed-code.md)。

若要在项目上手动运行代码分析，从菜单栏选择**分析** > **运行代码分析** > **对运行代码分析<project>** . 有关详细信息，请参阅[如何： 启用和禁用自动代码分析](../code-quality/how-to-enable-and-disable-automatic-code-analysis-for-managed-code.md)。

## <a name="rule-sets"></a>规则集

对于托管代码的代码分析规则划分到*规则集*。 可以使用某个 Microsoft 标准规则集，也可以创建自定义规则集以满足特定需求。 有关详细信息，请参阅[使用规则集组合代码分析规则](../code-quality/using-rule-sets-to-group-code-analysis-rules.md)。

## <a name="in-source-suppression"></a>在禁止显示源

它通常用于指示警告不适用。 这样，便可以通知开发人员以及可能会在以后检查代码的其他人员：已调查了一个警告，且禁止显示或忽略了该警告。

在源中的禁止显示警告实现通过自定义特性。 若要禁止显示警告，请向源代码添加特性 `SuppressMessage`，如下面的示例所示：

```csharp
[System.Diagnosis.CodeAnalysis.SuppressMessage("Microsoft.Design", "CA1039:ListsAreStrongTyped")]
Public class MyClass
{
   // code
}
```

有关详细信息，请参阅[禁止显示警告使用 SuppressMessage 特性](../code-quality/suppress-warnings-by-using-the-suppressmessage-attribute.md)。

## <a name="run-code-analysis-as-part-of-check-in-policy"></a>作为签入策略的一部分运行代码分析

作为一个单位，可能希望所有签入行为满足特定的策略。 特别是希望确保遵从下列策略：

- 签入代码中没有生成错误。

- 作为最新生成的一部分运行代码分析。

可以通过指定签入策略来实现该任务。 有关详细信息，请参阅[利用团队项目签入策略提高代码质量](../code-quality/enhancing-code-quality-with-team-project-check-in-policies.md)。

## <a name="team-build-integration"></a>Team build 集成

你可以使用生成系统的集成功能在生成过程中运行分析工具。 有关详细信息，请参阅[生成和发布 (VSTS)](/vsts/build-release/index)。

## <a name="see-also"></a>请参阅

[使用规则集组合代码分析规则](../code-quality/using-rule-sets-to-group-code-analysis-rules.md)   
[如何： 启用和禁用自动代码分析](../code-quality/how-to-enable-and-disable-automatic-code-analysis-for-managed-code.md)