---
title: "Visual Studio IDE 概述 | Microsoft Docs"
ms.custom: 
ms.date: 11/09/2017
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
author: gewarren
ms.author: gewarren
manager: ghogen
ms.workload: multiple
ms.openlocfilehash: d95cbaff8545e67bfadb0c86a256353b3fa23191
ms.sourcegitcommit: f9fbf1f55f9ac14e4e5c6ae58c30dc1800ca6cda
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/10/2018
---
# <a name="visual-studio-ide-overview"></a>Visual Studio IDE 概述

Visual Studio 交互式开发环境 (IDE) 是一种创新启动板，可用于查看和编辑几乎任何类型的代码，并调试、生成和发布适用于 Android、iOS、Windows、Web 和云的应用。 有适用于 Mac 和适用于 Windows 的版本。 本文介绍了 Visual Studio IDE 的功能。 本文介绍可通过 Visual Studio 执行的一些操作以及如何安装和使用 Visual Studio，我们会引导你创建一个简单的项目、提供有关调试和部署代码的指导并介绍各种工具窗口。

## <a name="what-can-you-do-with-the-visual-studio-ide"></a>你可以通过 Visual Studio IDE 做什么？

要创建一个适用于 Android 手机的应用？ 可以。 想使用 C++ 来创建一个热门游戏？ 也可以，此外还可以做很多其他事情。 Visual Studio 提供了各种模板，可以帮助你制作网站、游戏、桌面应用、移动应用和 Office 相关应用等。

![Visual Studio 项目](../ide/media/VSIDE_Tour_Projects_List.png)

或者，你只需打开从任何地方获取的一些代码即可开始处理。 在 GitHub 上看到了喜欢的项目？ 只需克隆存储库，在 Visual Studio 中将其打开，然后就可以开始编写代码！

### <a name="create-mobile-apps"></a>创建移动应用

可通过使用 Visual C# 和 Xamarin 或 Visual C++ 创建不同平台的本机移动应用，或者通过结合使用 JavaScript 和 Apache Cordova 创建混合应用。 可以编写适用于 Unity、Unreal、DirectX、Cocos 等的移动游戏。 Visual Studio 带有 Android 仿真程序，可以帮助你运行和调试 Android 应用。

可以创建 Azure 应用服务，将云的强大功能应用到移动应用。 通过 Azure 应用服务，应用可将数据存储在云端、安全地验证用户身份并自动缩放其资源以满足你的应用和业务需求。 有关详细信息，请参阅[移动应用开发](https://www.visualstudio.com/vs/mobile-app-development/)。

### <a name="create-cloud-apps-for-azure"></a>创建 Azure 云应用

通过 Visual Studio 提供的工具套件，可以轻松地创建由 Microsoft Azure 提供支持的云启用应用程序。 可以轻松地从 IDE 直接配置、构建、调试、打包和部署 Microsoft Azure 上的应用程序和服务。 若要获取用于 .NET 的 Azure 工具，安装 Visual Studio 时请选择“Azure 开发”工作负载。 有关详细信息，请参阅 [Visual Studio Tools for Azure](https://www.visualstudio.com/vs/azure-tools/)。

可以通过如下所示的连接的服务为应用使用 Azure 服务：

- [Azure 移动服务](http://azure.microsoft.com/documentation/services/mobile-services/)

- [Azure 存储](http://azure.microsoft.com/documentation/services/storage/)

[HockeyApp](https://www.visualstudio.com/hockey-app/) 有助于分发测试版本、收集实时故障报表和获取真实用户的反馈。 此外，可将 Office 365 REST API 集成到你自己的应用中，以连接到云中存储的数据。 有关详细信息，请参阅[这些 GitHub 示例](https://github.com/OfficeDev/?utf8=%E2%9C%93&query=o365)。

[Application Insights](https://marketplace.visualstudio.com/items?itemName=VisualStudioOnlineApplicationInsights.application-insights) 有助于检测和诊断应用和 Web 服务中的质量问题。 Application Insights 还有助于了解用户通过应用实际进行的操作，便于优化用户体验。

### <a name="create-apps-for-the-web"></a>创建 web 应用

Web 推动着现代社会前进，Visual Studio 可以帮助你编写 Web 应用。 可以使用 ASP.NET、Node.js、Python、JavaScript 和 TypeScript 来创建 Web 应用。 Visual Studio 了解 Angular、jQuery、Express 等 Web 框架。 ASP.NET Core 和 .NET Core 在 Windows、Mac 和 Linux 操作系统上运行。 [ASP.NET Core](http://www.asp.net/core/overview) 是 MVC、WebAPI 和 SignalR 的一个重大更新，并在 Windows、Mac 和 Linux 上运行。  ASP.NET Core 旨在完全为你提供可组合的精益 .NET 堆栈，以便生成基于云的新式 Web 应用和服务。

有关详细信息，请参阅[新式 Web 工具](https://www.visualstudio.com/vs/modern-web-tooling/)。

### <a name="build-cross-platform-apps-and-games"></a>生成跨平台应用和游戏

可使用 Visual Studio 生成适用于 Android、iOS 和 Linux 等设备的应用和游戏。 若要了解详细信息，请参阅[跨平台移动开发](../cross-platform/cross-platform-mobile-development-in-visual-studio.md)。 通用 Windows 应用可帮助在多个平台中利用代码。 有关详细信息，请参阅[通用 Windows 应用](https://dev.windows.com/en-us/windows-apps)。

基于应用要求和要使用的语言选择所需工具：

- [Xamarin for Visual Studio](../cross-platform/build-apps-with-native-ui-using-xamarin-in-visual-studio.md)：针对所有设备的 C# 中的常用基本代码。

- [Visual Studio Tools for Apache Cordova](../cross-platform/visual-studio-tools-for-apache-cordova.md)：适用于 HTML、CSS 和 JavaScript 或 Typescript 的常用基本代码。

- [Visual Studio Tools for Unity](../cross-platform/visual-studio-tools-for-unity.md)：C# 中的 2D/3D 游戏开发。

- [适用于跨平台开发的 C++](../cross-platform/visual-cpp-for-cross-platform-mobile-development.md)：C++ 中的共享代码库和应用。

- [适用于 Android 的 Visual Studio 模拟器](../cross-platform/visual-studio-emulator-for-android.md)：适用于 Android 的 Visual Studio 模拟器：调试和测试 Android 应用而无需考虑 IDE。

[使用 Visual Studio 创建游戏](https://www.visualstudio.com/vs/game-development/)，通过 DirectX、Unity、Unreal、Cocos 等游戏开发工具。

Visual Studio 能够帮助你实现更多操作。 有关更完整的列表，请参阅 [Visual Studio IDE](https://www.visualstudio.com/vs/)。

## <a name="install-the-visual-studio-ide"></a>安装 Visual Studio IDE

首先，请下载 Visual Studio 并将其安装到你的系统上。 可以在 [Visual Studio 2017](https://aka.ms/vsdownload?utm_source=mscom&utm_campaign=msdocs) 中进行下载。

Visual Studio 现在达到了前所未有的轻量！ 通过模块化安装程序，可以选择和安装工作负荷。工作负荷是你习惯使用的编程语言或平台所需的一些功能。 此策略使 Visual Studio 安装的占用空间比之前更小，这也意味着其安装和更新速度会更快。

若要执行以下程序创建步骤，请务必选择并安装“通用 Windows 平台开发”工作负荷。

![Visual Studio 安装程序](../ide/media/vside_tour_install_dialog.png)

除了安装性能的改进之外，Visual Studio 2017 的 IDE 启动时间和解决方案加载时间都更短。

若要了解设置系统上的 Visual Studio 的详细信息，请参阅[安装 Visual Studio 2017](../install/install-visual-studio.md)。

## <a name="sign-in"></a>登录

首次启动 Visual Studio 时，可选择使用 Microsoft 帐户或者单位或学校帐户登录。 登录后可以跨多个设备同步窗口布局等 Visual Studio 设置。 还能将你自动连接到你可能需要的服务，例如 Azure 订阅和 Visual Studio Team Services。

## <a name="create-a-program"></a>创建程序

学习的最好方式是动手操作！ 现在我们来深入了解并创建一个简单的新程序。

1. 打开 Visual Studio。 在菜单上，依次选择“文件”“新建”“项目”。

  ![屏幕截图](../ide/media/VSIDE_Tour_NewProject1.png)

  也可以使用起始页来新建项目。 有关详细信息，请参阅[借力于经重新设计的起始页（博文）](https://blogs.msdn.microsoft.com/visualstudio/2016/11/29/harness-the-power-of-the-redesigned-start-page/)。

1. “新建项目”对话框中会显示几个项目模板。 在“Visual C#”下选择“Windows Universal”类别，再选择“空白应用(通用 Windows)”模板，然后选择“确定”按钮。

  ![屏幕截图](../ide/media/VSIDE_Tour_NewProject2.png)

  此操作创建了一个新的空白 Universal Windows 应用项目，该项目使用 Visual C# 和 XAML 作为编程语言。 稍等片刻，等待 Visual Studio 设置项目。 如果系统出现任何信息提示，现在都接受默认值。

1. 在“新式通用 Windows 项目”对话框中，选择“确定”接受默认设置。

1. 稍后，你将看到类似于以下屏幕截图的内容。 右侧名为“解决方案资源管理器”的窗口中列出了你的项目文件。

  ![屏幕截图](../ide/media/VSIDE_Tour_NewProject3.png)

1. 在解决方案资源管理器中，选择 MainPage.xaml 文件旁边小的黑色三角形，将其展开，在下面应该可以看到一个 MainPage.xaml.cs 文件。 选择此文件（其中包含 C# 代码）将其打开。

  MainPage.xaml.cs 中的 C# 代码将出现在屏幕左侧的代码编辑器中。 请注意，已经自动将代码语法着色，以指示语句或注释等不同类型的代码。 此外，代码中的垂直短虚线指示哪两个大括号相匹配，行号能够帮助你在以后查找代码。 可以通过选择带减号的小方形来折叠或展开代码。 此代码大纲功能可以隐藏不需要的代码，最大程度地减少屏幕混乱。

  ![](../ide/media/VSIDE_Tour_NewProject3a.png)

  还提供了一些其他的菜单和工具窗口，但是现在我们继续下一步操作。

1. 在 XAML 窗体中添加按钮，让用户可以和你的应用交互。 若要执行此操作，请打开 MainPage.xaml 文件。 下面是一个拆分视图：上面是一个可以直观放置控件的设计器，下面是一个代码视图，代码视图中显示了设计器对应的 XAML 代码。 以后运行该程序时，设计器中的内容会成为用户将看到的窗口，即一个“窗体”，并且窗体上显示的内容由基础 XAML 决定。

1. 在屏幕左侧，选择“工具箱”选项卡以打开工具箱。 工具箱中有许多可以添加到窗体的可视化控件。 现在我们只添加一个按钮控件。

1. 展开“常用 XAML 控件”部分，然后将按钮控件拖动到窗体的大概中间位置。 （位置的准确性并不重要。）

  ![屏幕截图](../ide/media/VSIDE_Tour_Toolbox.png)

  完成后，应该看到类似于以下屏幕截图的内容。

  ![屏幕截图](../ide/media/VSIDE_Tour_XAMLButton.png)

  按钮位于设计器上，其基础代码（高亮显示）被自动添加到了设计器的 XAML 代码中。

1. 我们对 XAML 代码进行一些更改。 将按钮代码中的文本从 `Button` 重命名为 `Hello!`。

  ![屏幕截图](../ide/media/VSIDE_Tour_XAMLButton2.png)

1. 现在启动该应用。 可以通过选择工具栏上的“启动”（![启动按钮](../ide/media/VSIDE_StartButton.png)），或按 F5，或者在菜单中依次选择“调试”、“开始调试”来实现此操作。

  ![屏幕截图](../ide/media/VSIDE_Tour_RunButton.png)

  应用将开始其生成过程，并且会在输出窗口中显示状态消息。 不久后应显示窗体，并且你添加的按钮在该窗体上。 现在你拥有了一个正在运行的应用！

  ![屏幕截图](../ide/media/VSIDE_Tour_RunProject.png)

  当然，现在它还不能实现太多功能，但是如果你愿意，可以稍后为其添加更多功能。

1. 该程序运行完毕后，选择工具栏上的“停止”（![“停止”按钮](../ide/media/VSIDE_StopButton.png)）按钮来使其停止。

我们来回顾一下到目前为止的操作：在 Visual Studio 中新建一个 C# Windows Universal 项目、查看该项目的代码、在设计器中添加一个控件、更改某些 XAML 代码，然后运行该项目。 虽然本示例中的流程经过简化，但它为你展示了开发自己的应用时一些常用的 Visual Studio IDE 部件。 如需有关此示例的详细信息，请参阅[创建一个“Hello, world”应用 (XAML)](/windows/uwp/get-started/create-a-hello-world-app-xaml-universal)。

## <a name="debug-test-and-improve-your-code"></a>调试、测试和改进代码

没有始终可以完美运行的应用。 编写代码时，需要运行并测试该代码以了解 bug 和性能。 使用 Visual Studio 先进的调试系统，可以调试在本地项目、远程设备或仿真程序（例如 Android 或 Windows Phone 设备的仿真程序）上运行的代码。 可以一次一个语句逐行执行代码并随时检查变量，可以逐行执行多个线程应用程序，还可以设置只在特定条件为“真”时才命中的断点。 代码运行时可以监视变量的值等。 上述所有操作均可在代码编辑器中管理，因此无需离开代码。

![调试](../ide/media/VSIDE_Tour_Debugging.png)

针对测试，Visual Studio 提供了单元测试、IntelliTest、负载和性能测试等。 有关 Visual Studio 调试过程的详细信息，请参阅[调试器功能简介](../debugger/debugger-feature-tour.md)。 有关测试的详细信息，请参阅[测试工具和方案](../test/developer-testing-scenarios.md)。 有关提升应用性能的详细信息，请参阅[分析功能导览](../profiling/profiling-feature-tour.md)。

## <a name="deploy-your-finished-application"></a>部署完成的应用程序

当应用程序可以部署给用户或客户时，无论是部署到 Microsoft Store 还是 SharePoint 站点，无论是通过 InstallShield 还是 Windows Installer 技术进行部署，Visual Studio 都会提供实现此操作的工具。 这些都可以通过 IDE 进行访问。 有关详细信息，请参阅[部署应用程序、服务和组件](../deployment/deploying-applications-services-and-components.md)。

## <a name="quick-tour-of-the-ide"></a>IDE 快速教程

为了向你提供有关 Visual Studio 的高级直观概览，下图显示了在 Visual Studio 中打开的一个项目，以及你最有可能用到的几个关键工具窗口：

- [解决方案资源管理器](../ide/solutions-and-projects-in-visual-studio.md)可让你查看、导航和管理代码文件。 解决方案资源管理器可将代码文件分组为解决方案和项目，从而帮助整理代码。

- [编辑器](../ide/writing-code-in-the-code-and-text-editor.md)窗口显示代码，可通过该窗口编辑源代码和设计 UI，此处你可能会花费大部分时间。

- [输出](../ide/reference/output-window.md)窗口是 Visual Studio 发送通知（例如，调试和错误消息、编译器警告、发布状态消息等）的位置。 每个消息源都有自己的选项卡。

- 利用版本控制技术（如 [Git](https://git-scm.com/) 和 [Team Foundation 版本控制 (TFVC)](/vsts/tfvc/overview)），[团队资源管理器 (VSTS)](/vsts/user-guide/work-team-explorer) 可让你跟踪工作项并与他人共享代码。

- [Cloud Explorer](/azure/vs-azure-tools-resources-managing-with-cloud-explorer) 可让你查看和管理 Azure 资源，如虚拟机、表格以及 SQL 数据库等。 如果某一特定操作需要 Azure 门户，Cloud Explorer 会提供你在 Azure 门户中所需位置的链接。

![Visual Studio IDE](../ide/media/visualstudioide.png)

下面是 Visual Studio 中其他一些常见的工作效率功能：

- 使用[快速启动](../ide/reference/quick-launch-environment-options-dialog-box.md)搜索框可以在 Visual Studio 中快速找到所需内容。 只需输入要查找内容的名称，Visual Studio 就会为你列出结果，这些结果可以准确地将你导向目标位置。 “快速启动”还可以显示链接，这些链接可以启动任何工作负载或单个组件的 Visual Studio 安装程序。

  ![“快速启动”搜索框](../ide/media/VSIDE_Tour_QuickLaunch.png)

- [重构](../ide/refactoring-in-visual-studio.md)包括智能重命名变量、移动选定的代码行到单独的函数、移动代码到其他位置、重新排序函数参数以及更多操作。

 ![重构](../ide/media/VSIDE_refactor.png)

- “IntelliSense”是一组常用功能的涵盖性术语，这些功能可用于在编辑器中直接显示代码的类型信息，并且可在某些情况下编写小段代码。 如同在编辑器中拥有了基本文档内联，从而节省了在单独帮助窗口查看类型信息的时间。 IntelliSense 功能因语言而异。 有关详细信息，请参阅 [Visual C# IntelliSense](../ide/visual-csharp-intellisense.md)、[Visual C++ Intellisense](../ide/visual-cpp-intellisense.md)、[JavaScript IntelliSense](../ide/javascript-intellisense.md) 和 [Visual Basic 特定的 IntelliSense](../ide/visual-basic-specific-intellisense.md)。 下图显示了一些处于工作状态的 IntelliSense 功能：

  ![Visual Studio 成员列表](../ide/media/vs2017_Intellisense.png)

- **波形曲线**是红色的波浪形下划线，它可以在你键入时实时警告你注意代码中的错误或者潜在问题。 这样一来，你可立即修复错误，而无需等到编译或运行时才发现错误。 如果将鼠标悬停在波形曲线上，将看到关于此错误的其他信息。 左边距上也可能会出现一个灯泡，提供有关如何修复此错误的建议。 有关详细信息，请参阅[快速操作](../ide/quick-actions.md)。

 ![波形曲线](../ide/media/vs2017_squiggle.png)

- 可以在文本编辑器上下文菜单中打开[调用层次结构](../ide/reference/call-hierarchy.md)窗口，以显示调用方法、被调用方法和插入点下的方法（插入点）。

 ![“调用层次结构”窗口](../ide/media/VSIDE_call_hierarchy.png)

- [“CodeLens”](../ide/find-code-changes-and-other-history-with-codelens.md)能够查找代码引用、代码更改、链接错误、工作项、代码评审和单元测试，所有操作都在编辑器上进行。

 ![CodeLens](../ide/media/codelensoverview.png)

- [“查看定义”](../ide/how-to-view-and-edit-code-by-using-peek-definition-alt-plus-f12.md) 窗口显示方法或类型的定义内联，而无需离开当前的上下文。

 ![查看定义](../ide/media/VSIDE_peek_definition.png)

- “转到定义”  上下文菜单选项可直接进入其中定义函数或对象的位置。 还可以在编辑器中右键单击来获取其他导航命令。

 ![转到定义](../ide/media/VSIDE_go_to_definition.png)

- [对象浏览器](http://msdn.microsoft.com/f89acfc5-1152-413d-9f56-3dc16e3f0470)，作为相关的工具，可以检查系统上的 .NET 或 Windows 运行时程序集，以查看其中包含的类型以及这些类型包含的成员（属性、方法、事件等）。

  ![显示 System.Timer 的对象浏览器](../ide/media/objectbrowser.png)

## <a name="manage-your-source-code-and-collaborate-with-others"></a>管理源代码并与他人协作

可以在任意提供商（包括 GitHub）托管的 Git 存储库中管理源代码。 或者，使用 [Visual Studio Team Services (VSTS)](/vsts/index) 管理整个项目的代码、Bug 和工作项。 若要详细了解如何在 Visual Studio 中使用团队资源管理器管理 Git 存储库，请参阅[开始使用 Git 和 Team Services (VSTS)](/vsts/git/gitquickstart?tabs=visual-studio)。 Visual Studio 还内置有其他源代码管理功能。 若要了解详细信息，请参阅 [Visual Studio 2017 中的新 Git 功能（博文）](https://blogs.msdn.microsoft.com/visualstudioalm/2017/03/06/new-git-features-in-visual-studio-2017/)。

Visual Studio Team Services 是一种基于云的服务，用于承载软件项目和启用团队中的协作。 VSTS 支持 Git 和 Team Foundation 源控件系统以及 Scrum、CMMI 和 Agile 开发方法。 Team Foundation 版本控制 (TFVC) 采用单一的集中式服务器存储库来跟踪文件和调整它的版本。 本地更改始终签入到中央服务器，其他开发人员可在此处获得最新的更改。

Team Foundation Server (TFS) 是 Visual Studio 的应用程序生命周期管理中心。 它使用单个解决方案，使开发过程中涉及的所有人均可参与该开发过程。 TFS 对于管理异类团队和项目也非常有用。

如果你的网络中已经具有 Visual Studio Team Services 帐户或 Team Foundation Server，则可通过 Visual Studio 中的“团队资源管理器”窗口连接。 可在此窗口中将代码签入（出）源控件、管理工作项、启动生成以及访问团队聊天室和工作区。 可以从“快速启动”框，或者“视图，团队资源”或“团队，管理连接”的主菜单中打开“团队资源管理器”。

下图展示了 VSTS 中托管的解决方案的“团队资源管理器”窗口。

![Visual Studio 团队资源管理器](../ide/media/vs2017_teamexplorer.png)

还可以自动执行生成过程以生成团队中的开发人员签入到版本控制的代码。 例如，您可以在夜间或每次签入此代码时生成一个或多个项目。 有关详细信息，请参阅 [Continuous integration on any platform](https://www.visualstudio.com/en-us/docs/build/overview)（任何平台上的持续集成）。

## <a name="connect-to-services-databases-and-cloud-based-resources"></a>连接到服务、数据库和基于云的资源

云对当今的联机环境至关重要，Visual Studio 为你提供了利用云的方法。 例如，连接的服务功能可以将应用与服务相连接。 应用可以通过该功能将其数据存储到 Azure 存储。

![连接的服务](../ide/media/VSIDE_Tour_Connected_Services.png)

在“连接的服务”页上选择一个服务可以启动“连接的服务向导”，该向导会配置项目、下载必要的 NuGet 数据包，从而帮助你根据服务需要进行编码。

可以通过使用 [Cloud Explorer](/azure/vs-azure-tools-resources-managing-with-cloud-explorer) 来查看和管理 Visual Studio 中基于 Azure 的云资源。 Cloud Explorer 可以显示你登录的 Azure 订阅下托管的所有帐户中的 Azure 资源。 在 Visual Studio 安装程序中选择“Azure 开发”工作负载即可获取 Cloud Explorer。

![Cloud Explorer](../ide/media/VSIDE_CloudExplorer.png)

服务器资源管理器有助于你浏览和管理本地、远程以及 Azure、Salesforce.com、Office 365 和网站上的 SQL Server 实例及资产。 若要打开“服务器资源管理器”，请在主菜单上依次选择“视图”、“服务器资源管理器”。 请参阅[添加新连接](../data-tools/add-new-connections.md)，了解有关使用服务器资源管理器的详细信息。

[SQL Server Data Tools (SSDT)](/sql/ssdt/download-sql-server-data-tools-ssdt) 是一个适用于 SQL Server、Azure SQL 数据库和 Azure SQL 数据仓库的强大的开发环境。 通过它可以生成、调试、维护和重构数据库。 可使用数据库项目，或直接使用已连接的数据库实例（本地或非本地）。

Visual Studio 中的 **SQL Server 对象资源管理器**提供类似于 SQL Server Management Studio 中的数据库对象。 使用 SQL Server 对象资源管理器可以执行轻负载数据库管理和设计工作，包括使用 SQL Server 对象资源管理器右侧的上下文菜单编辑表数据、对比架构和执行查询等。

![SQL Server 对象资源管理器](../ide/media/vs2015_sqlobjectexplorer.png)

## <a name="extend-visual-studio"></a>扩展 Visual Studio
如果 Visual Studio 中没有你需要的确切功能，你可以进行添加！ 可以根据你的工作流和风格自定义 IDE，对尚未与 Visual Studio 集成的外部工具添加支持并修改现有的功能，以提高工作效率。 若要查找 Visual Studio 扩展性工具 (VS SDK) 的最新版本，请参阅 [Visual Studio SDK](../extensibility/visual-studio-sdk.md)。

可以使用 .NET Compiler Platform (Roslyn) 编写自己的代码分析器和代码生成器。 在 [Roslyn](https://github.com/dotnet/Roslyn)中查找所需的一切内容。

查找由 Microsoft 开发人员以及我们的开发社区创建的 Visual Studio [现有扩展](https://marketplace.visualstudio.com/vs)。

若要了解有关扩展 Visual Studio 的详细信息，请参阅[扩展 Visual Studio IDE](https://www.visualstudio.com/vs/extend/)。

## <a name="learn-more-and-find-out-whats-new"></a>了解详细信息和新增功能

如果之前从未用过 Visual Studio，请查看 [Visual Studio 开发入门](../ide/get-started-developing-with-visual-studio.md)，或观看 [Microsoft Virtual Academy](https://mva.microsoft.com/product-training/visual-studio-courses#!index=2&lang=1033) 上的 Visual Studio 免费课程。 若要了解 Visual Studio 2017 的新增功能，请参阅 [Visual Studio 2017 中的新增功能](../ide/whats-new-in-visual-studio.md)。

恭喜你，你已经完成了 Visual Studio IDE 课程！ 希望你已经对 Visual Studio 的一些主要功能有所了解。

## <a name="see-also"></a>请参阅

* [Visual Studio IDE](https://www.visualstudio.com/vs/)
* [Visual Studio 下载](https://www.visualstudio.com/downloads/)
* [Visual Studio 博客](https://blogs.msdn.microsoft.com/visualstudio/)
* [Visual Studio 论坛](https://social.msdn.microsoft.com/Forums/vstudio/en-US/home?category=visualstudio%2Cvsarch%2Cvsdbg%2Cvstest%2Cvstfs%2Cvsdata%2Cvsappdev%2Cvisualbasic%2Cvisualcsharp%2Cvisualc)
* [Microsoft 虚拟学院](https://mva.microsoft.com/)
* [第 9 频道](https://channel9.msdn.com/)
