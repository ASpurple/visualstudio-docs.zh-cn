---
title: "如何在 Visual Studio 中使用适用于 C++ 的 CTest | Microsoft Docs"
ms.custom: 
ms.date: 11/07/2017
ms.reviewer: 
ms.suite: 
ms.technology: vs-devops-test
ms.tgt_pltfrm: 
ms.topic: article
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
author: mikeblome
ms.openlocfilehash: 989f2b06df55fd0927863fe7e5603d3d0ec90b06
ms.sourcegitcommit: 7ae502c5767a34dc35e760ff02032f4902c7c02b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2018
---
# <a name="how-to-use-ctest-for-c-in-visual-studio"></a>如何在 Visual Studio 中使用适用于 C++ 的 CTest
CMake（包括 CTest）作为“使用 C++ 的桌面开发”工作负荷的组件集成到 Visual Studio IDE 中。 若要在计算机上安装它，请打开 Visual Studio 安装程序，在工作负荷组件列表下找到[Visual C++ 的 CMake 工具](/cpp/ide/cmake-tools-for-visual-cpp)。

Visual Studio 中的 CMake 支持不涉及 Visual Studio 项目系统。 因此，可如同在任何 CMake 环境中一样编写和配置 CTest 测试。 有关在 Visual Studio 中使用 CMake 的详细信息，请参阅 [Visual C++ 的 CMake 工具](/cpp/ide/cmake-tools-for-visual-cpp)。

Visual Studio 2017 版本 15.5 CTest 当前未与“测试资源管理器”集成。 可以从 CMake 主菜单，或是在“解决方案资源管理器”中从 CMakeLists.txt 文件的上下文菜单运行测试。 测试结果会定向到 Visual Studio 输出窗口。

![运行 CTest 测试](media/cpp-cmake-run-tests.png "Run CTest tests")


## <a name="see-also"></a>请参阅
[编写 C/C++ 单元测试](writing-unit-tests-for-c-cpp.md)


  







