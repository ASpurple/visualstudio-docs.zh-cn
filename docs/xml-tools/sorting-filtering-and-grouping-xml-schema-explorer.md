---
title: "排序、 筛选和分组 （XML 架构资源管理器） |Microsoft 文档"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: vs-ide-general
ms.tgt_pltfrm: 
ms.topic: article
ms.assetid: 4a914de0-9ffc-4526-9603-92e460e52513
caps.latest.revision: "2"
author: gewarren
ms.author: gewarren
manager: ghogen
ms.workload: multiple
ms.openlocfilehash: b8fe3daa1c95169623a908307d4d6c81044d378f
ms.sourcegitcommit: 32f1a690fc445f9586d53698fc82c7debd784eeb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2017
---
# <a name="sorting-filtering-and-grouping-xml-schema-explorer"></a>排序、筛选和分组（XML 架构资源管理器）
本主题介绍了可通过选项**排序、 筛选和分组选项**XML 架构资源管理器工具栏上的菜单。  
  
## <a name="filter-options"></a>筛选器选项  
 下列筛选器选项可用。 默认情况下，**显示命名空间**和**显示架构文件**会选择的选项。  
  
-   **显示命名空间**。  
  
-   **显示架构文件**。  
  
-   **显示排序器 （序列/选项/全部）**。  
  
## <a name="sorting-options"></a>排序选项  
 下列排序选项可用。 默认值是**按类型排序**。 “排序方式”选项不适用于文件和命名空间。  
  
-   **按类型排序**。  
  
-   **按名称排序**。  
  
-   **文档顺序**。  
  
### <a name="sort-by-type"></a>按类型排序  
 当**按类型排序**选择选项后，全局节点按以下顺序进行排序。 然后，节点将在每个组中按字母顺序进行排序。  
  
1.  `import` 节点。  
  
2.  `include` 节点。  
  
3.  `redefine` 节点。  
  
4.  `attribute` 节点。  
  
5.  `attributeGroup` 节点。  
  
6.  `complexType` 节点。  
  
7.  `simpleType` 节点。  
  
8.  `element` 节点。  
  
9. `group` 节点。  
  
### <a name="sort-by-name"></a>按名称排序  
 当**按名称排序**选择选项后，全局节点进行排序顺序如下：  
  
1.  `import` 节点（按命名空间的字母顺序）。  
  
2.  `include` 节点（按 `schemaLocation` 特性的字母顺序）。  
  
3.  `redefine` 节点（按 `schemaLocation` 特性的字母顺序）。  
  
4.  其他全局节点（按字母顺序）。  
  
### <a name="document-order"></a>文档顺序  
 **文档顺序**时，选项才可用**显示架构文件**选项。 当**文档顺序**选择后，全局节点的架构文件中出现的顺序显示。  
  
## <a name="persisting-sortfilter-options"></a>保留排序/筛选器选项  
 无论更改设置时打开的是哪个解决方案或文件，排序、筛选和分组选项均会保存到每个用户的注册表中。