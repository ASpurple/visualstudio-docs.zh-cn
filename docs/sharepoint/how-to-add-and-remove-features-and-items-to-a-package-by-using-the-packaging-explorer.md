---
title: "如何： 添加和移除功能和包项使用打包资源管理器 |Microsoft 文档"
ms.custom: 
ms.date: 02/02/2017
ms.reviewer: 
ms.suite: 
ms.technology: office-development
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: VS.SharePointTools.RAD.PackagingExplorer
dev_langs:
- VB
- CSharp
- VB
- CSharp
helpviewer_keywords: SharePoint development in Visual Studio, packages
author: TerryGLee
ms.author: tglee
manager: ghogen
ms.workload: office
ms.openlocfilehash: 25a2514f2d25661de2898be8d2ef9ff051cc5559
ms.sourcegitcommit: f9fbf1f55f9ac14e4e5c6ae58c30dc1800ca6cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/10/2018
---
# <a name="how-to-add-and-remove-features-and-items-to-a-package-by-using-the-packaging-explorer"></a>如何：使用打包资源管理器在包中添加和移除功能和项
  若要配置包以部署 SharePoint 项和功能，可以使用打包资源管理器。 .Wsp 文件中，你可以调整的 SharePoint 项目项和功能。  
  
 或者，你可以使用打包设计器查看和重新排序的功能，若要更改激活顺序。 有关详细信息，请参阅[如何： 添加和删除通过使用包设计器的功能和包项](../sharepoint/how-to-add-and-remove-features-and-items-to-a-package-by-using-the-package-designer.md)。  
  
## <a name="opening-the-packaging-explorer"></a>打开打包资源管理器  
 你可以使用以下过程打开打包资源管理器，如果你的 Visual Studio 解决方案有至少一个 SharePoint 项目。 或者，打包资源管理器将自动打开时查看功能或包设计器。 关闭所有功能和包设计器后，打包资源管理器也会关闭。  
  
#### <a name="to-open-the-packaging-explorer"></a>若要打开打包资源管理器  
  
1.  在菜单栏上，选择**视图**，**其他窗口**，**打包资源管理器**。  
  
     **打包资源管理器**出现在**工具箱**。  
  
## <a name="adding-a-feature-to-a-package"></a>将功能添加到包  
 通过使用打包资源管理器，可以向包添加新的和现有功能。  
  
#### <a name="to-add-a-sharepoint-feature"></a>若要添加 SharePoint 功能  
  
1.  打开**打包资源管理器**，打开该项目的快捷菜单，然后选择**添加功能**。  
  
#### <a name="to-move-an-existing-sharepoint-feature"></a>若要移动现有的 SharePoint 功能  
  
1.  打开**打包资源管理器**，然后执行以下步骤之一：  
  
    -   拖动**功能**到另一个项目的不同项目中。  
  
    -   对于每项功能打开快捷菜单，选择**剪切**，打开你想要移动该功能，然后选择的项目的快捷菜单**粘贴**。  
  
    > [!NOTE]  
    >  如果解决方案中包含多个 SharePoint 项目，请使用此过程。  
  
## <a name="validating-a-feature-or-package"></a>验证功能或包  
 可以通过验证文件来识别中的 SharePoint 功能和包的潜在问题。 警告和错误将显示在输出窗口和错误列表窗口中。  
  
#### <a name="to-validate-a-sharepoint-feature-or-package"></a>若要验证的 SharePoint 功能或包  
  
1.  打开**打包资源管理器**。  
  
2.  功能或包，打开快捷菜单，然后选择**验证**。  
  
## <a name="see-also"></a>请参阅  
 [打包和部署 SharePoint 解决方案](../sharepoint/packaging-and-deploying-sharepoint-solutions.md)  
  
  