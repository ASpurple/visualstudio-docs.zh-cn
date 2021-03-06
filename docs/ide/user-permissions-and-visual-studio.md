---
title: "用户权限与 Visual Studio | Microsoft Docs"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: vs-ide-general
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords:
- Visual Studio, user permissions
- user permissions
- administrative privileges
- permissions
ms.assetid: 70485ed7-6342-41bf-8250-7a6826e21b98
caps.latest.revision: "14"
author: gewarren
ms.author: gewarren
manager: ghogen
ms.workload: multiple
ms.openlocfilehash: 3cf223b0b4d2f8ca710a5d5fdb349c7a423b1b86
ms.sourcegitcommit: 32f1a690fc445f9586d53698fc82c7debd784eeb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="user-permissions-and-visual-studio"></a>用户权限与 Visual Studio
出于安全目的，你应尽可能以普通用户的身份来运行 Visual Studio。  

> [!WARNING]
>  你还应确保不要编译、启动或调试任何来自不受信任用户或地址的 Visual Studio 解决方案。  

 作为普通用户，你可以在 Visual Studio IDE 中完成几乎所有操作，但你需要管理员权限才能完成以下任务：  

|区域|任务|更多相关信息|  
|----------|----------|--------------------------|  
|安装|安装 Visual Studio。|[安装 Visual Studio](../install/install-visual-studio.md)|  
||安装、更新或移除本地 Help 内容。|[安装和管理本地内容](../ide/install-and-manage-local-content.md)|  
|应用程序类型|部署 SharePoint 的解决方案。|[开发 SharePoint 解决方案的需求](/office-dev/office-dev/requirements-for-developing-sharepoint-solutions)|  
||获取 [!INCLUDE[win8_appstore_long](../debugger/includes/win8_appstore_long_md.md)]的开发人员许可证。|[获取开发人员许可证](http://go.microsoft.com/fwlink/?LinkID=241313)|  
|工具箱|将经典 COM 控件添加到“工具箱”。|[使用工具箱](../ide/using-the-toolbox.md)|  
|外接程序|安装和使用通过使用 IDE 中的经典 COM 编写的加载项。|[创建外接程序和向导](http://msdn.microsoft.com/Library/c5a47c21-6668-4de3-898d-afa969317e73)|  
|生成|使用注册组件的后期生成事件。|[了解自定义生成步骤和生成事件](/cpp/ide/understanding-custom-build-steps-and-build-events)|  
||在生成 C++ 项目时包括一个注册步骤。|[了解自定义生成步骤和生成事件](/cpp/ide/understanding-custom-build-steps-and-build-events)|  
|调试|调试使用提升的权限运行的应用程序。|[调试器设置和准备](../debugger/debugger-settings-and-preparation.md)|  
||调试在其他用户帐户下运行的应用程序，例如 ASP.NET 网站。|[调试 ASP.NET 和 AJAX 应用程序](../debugger/debugging-aspnet-and-ajax-applications.md)|  
||在区域中调试 XAML 浏览器应用程序 (XBAP)。|[WPF 主机 (PresentationHost.exe)](/dotnet/framework/wpf/app-development/wpf-host-presentationhost-exe)|  
||使用模拟器可以调试 Microsoft Azure 的云服务项目。|[在 Visual Studio 中调试云服务](http://go.microsoft.com/fwlink/?LinkId=266725)|  
||配置远程调试的防火墙。|[远程调试](../debugger/remote-debugging.md)|  
|性能工具|分析应用程序。|[性能分析初学者指南](../profiling/beginners-guide-to-performance-profiling.md)|  
|部署|在本地计算机上将 Web 应用程序部署到 Internet Information Services (IIS)。|[使用 Visual Studio 或 Visual Web Developer 将 ASP.NET Web 应用程序部署到承载提供程序：作为测试环境部署到 IIS](http://go.microsoft.com/fwlink/?LinkId=266478)|

## <a name="running-visual-studio-as-an-administrator"></a>以管理员身份运行 Visual Studio  
 每次启动 IDE 时，可利用管理权限启动 Visual Studio，或可以修改应用程序快捷方式以便始终利用管理权限运行。 有关详细信息，请参阅 Windows 帮助。  

#### <a name="to-run-visual-studio-with-administrative-permissions-on-includewin8debuggerincludeswin8mdmd-includewin81debuggerincludeswin81mdmd-includewinserver8debuggerincludeswinserver8mdmd-or-includewinblueserver2ideincludeswinblueserver2mdmd"></a>在 [!INCLUDE[win8](../debugger/includes/win8_md.md)]、[!INCLUDE[win81](../debugger/includes/win81_md.md)]、[!INCLUDE[winserver8](../debugger/includes/winserver8_md.md)] 或 [!INCLUDE[winblue_server_2](../ide/includes/winblue_server_2_md.md)]上利用管理权限运行 Visual Studio  

1.  在“开始”屏幕上，键入“Visual Studio”。 你应会看到你所安装的一个或多个 Visual Studio 版本。  

2.  选择要启动的 Visual Studio 版本，然后调出快捷菜单（显示在屏幕底部）。 选择 **“以管理员身份运行”**。  

     Visual Studio 启动时，标题栏的产品名后显示“(管理员)”。  

#### <a name="to-run-visual-studio-with-administrative-permissions-on-includewin7debuggerincludeswin7mdmd-or-includewinsvr08r2debuggerincludeswinsvr08r2mdmd"></a>在 [!INCLUDE[win7](../debugger/includes/win7_md.md)] 或 [!INCLUDE[winsvr08_r2](../debugger/includes/winsvr08_r2_md.md)] 上利用管理权限运行 Visual Studio  

1.  在“开始”菜单上，选择“所有程序”。  

2.  在 **Microsoft Visual Studio** 版本文件夹中，选择 **Visual Studio** 版本，打开快捷菜单，然后选择“以管理员身份运行”。  

     Visual Studio 启动时，标题栏的产品名后显示“(管理员)”。  

## <a name="see-also"></a>请参阅  
 [移植、迁移和升级 Visual Studio 项目](../porting/port-migrate-and-upgrade-visual-studio-projects.md)   
 [安装 Visual Studio](../install/install-visual-studio.md)
