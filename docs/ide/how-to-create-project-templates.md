---
title: "创建 Visual Studio 的项目模板 | Microsoft Docs"
ms.custom: 
ms.date: 01/02/2018
ms.reviewer: 
ms.suite: 
ms.technology: vs-ide-general
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: VS.ExportTemplateWizard
helpviewer_keywords: project templates [Visual Studio], creating
author: gewarren
ms.author: gewarren
manager: ghogen
ms.openlocfilehash: 0da7a7979b4fed6f58cdda6f1eafa55517e4df9b
ms.sourcegitcommit: 9357209350167e1eb7e50b483e44893735d90589
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2018
---
# <a name="how-to-create-project-templates"></a>如何：创建项目模板

本主题介绍如何使用“导出模板向导”创建模板，将模板打包为 .zip 文件。

## <a name="to-create-a-user-project-template-by-using-the-export-template-wizard"></a>使用“导出模板向导”创建用户项目模板

1. 创建项目。

    > [!NOTE]
    > 如果命名的项目将成为模板的源，则只使用有效的标识符字符。 否则，从模板创建的项目中可能发生编译错误。 有关有效标识符字符的详细信息，请参阅[已声明的元素名称 (Visual Basic)](/dotnet/visual-basic/programming-guide/language-features/declared-elements/declared-element-names) 或[标识符 (C++)](/cpp/cpp/identifiers-cpp)。 或者，可使用[模板参数](../ide/template-parameters.md)为类和命名空间使用“安全”名称。

1. 编辑项目，直到可以将它导出为一个模板。 例如，可能需要编辑代码文件以指出应替换参数的位置。 请参阅[如何：替换模板中的参数](../ide/how-to-substitute-parameters-in-a-template.md)。

1. 在“项目”菜单上，选择“导出模板”。

   “导出模板向导”随即打开。

1. 在“选择模板类型”页上，选择“项目模板”。 选择要导出到模板的项目，然后选择“下一步”。

1. 在“选择模板选项”页上，输入模板的名称和可选说明、图标和预览图像。 这些项将出现在“新建项目”对话框中。 选择“完成”。

  项目会导出到一个 .zip 文件中，并放在指定的输出位置，还可以导入到 Visual Studio（如果选择）。

>[!NOTE]
> 若要在“新建项目”对话框中找到模板，请展开“已安装”，然后展开 .vstemplate 文件中与 `ProjectType` 元素对应的类别。 例如，默认情况下，包含 `<ProjectType>CSharp</ProjectType>` 的 .vstemplate 文件显示在“已安装” > “Visual C#”下。 可将模板组织到项目类型的子目录中，只需在该目录中创建一个文件夹，然后将模板的 .zip 文件放入其中即可。 有关详细信息，请参阅[如何：查找和组织模板](../ide/how-to-locate-and-organize-project-and-item-templates.md)。

## <a name="other-ways-to-create-project-templates"></a>创建项目模板的其他方法

可通过将构成项目的文件收集到一个文件夹中来手动创建项目模板，然后使用适当的元数据创建 .vstemplate XML 文件。 有关详细信息，请参阅[如何：手动创建 Web 模板](../ide/how-to-manually-create-web-templates.md)。

如果已安装 Visual Studio SDK，可以使用“VSIX 项目”模板将完成的模板包装到 VSIX 文件中，供部署使用。 有关详细信息，请参阅 [VSIX 项目模板入门](../extensibility/getting-started-with-the-vsix-project-template.md)。

## <a name="see-also"></a>请参阅

[创建项目和项模板](../ide/creating-project-and-item-templates.md)  
[如何：创建项模板](../ide/how-to-create-item-templates.md)  
[VSIX 项目模板入门](../extensibility/getting-started-with-the-vsix-project-template.md)
