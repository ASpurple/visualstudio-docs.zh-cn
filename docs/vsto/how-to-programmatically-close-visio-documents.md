---
title: "如何： 以编程方式关闭 Visio 文档 |Microsoft 文档"
ms.custom: 
ms.date: 02/02/2017
ms.reviewer: 
ms.suite: 
ms.technology: office-development
ms.tgt_pltfrm: 
ms.topic: article
dev_langs:
- VB
- CSharp
helpviewer_keywords:
- documents [Office development in Visual Studio], closing Visio documents
- Visio [Office development in Visual Studio], closing Visio documents
author: TerryGLee
ms.author: tglee
manager: ghogen
ms.workload: office
ms.openlocfilehash: 090ba1dae3e870f5864455685c55092eac87f4df
ms.sourcegitcommit: f9fbf1f55f9ac14e4e5c6ae58c30dc1800ca6cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/10/2018
---
# <a name="how-to-programmatically-close-visio-documents"></a>如何：以编程方式关闭 Visio 文档
  你可以通过使用 Microsoft.Office.Interop.Visio.Document.Close 方法关闭活动 Microsoft Office Visio 文档。  
  
 有关此方法的详细信息，请参阅 [Microsoft.Office.Interop.Visio.Document.Close](http://msdn.microsoft.com/library/office/ff767415.aspx) 方法的 VBA 参考文档。  
  
## <a name="closing-the-active-document"></a>关闭活动文档  
  
#### <a name="to-close-the-active-document"></a>关闭活动文档  
  
-   调用 Microsoft.Office.Interop.Visio.Document.Close 方法关闭活动文档。  
  
     若要使用以下代码示例，请在 Visio 的 VSTO 外接程序项目内的 `ThisAddIn` 类中运行它。  
  
     [!code-csharp[Trin_VstcoreVisioAutomationAddIn#7](../vsto/codesnippet/CSharp/trin_vstcorevisioautomationaddin/ThisAddIn.cs#7)]
     [!code-vb[Trin_VstcoreVisioAutomationAddIn#7](../vsto/codesnippet/VisualBasic/trin_vstcorevisioautomationaddin/ThisAddIn.vb#7)]  
  
## <a name="see-also"></a>请参阅  
 [Visio 解决方案](../vsto/visio-solutions.md)   
 [Visio 对象模型概述](../vsto/visio-object-model-overview.md)   
 [如何： 以编程方式创建新的 Visio 文档](../vsto/how-to-programmatically-create-new-visio-documents.md)   
 [如何： 以编程方式打开 Visio 文档](../vsto/how-to-programmatically-open-visio-documents.md)   
 [如何： 以编程方式保存 Visio 文档](../vsto/how-to-programmatically-save-visio-documents.md)   
 [如何：以编程方式打印 Visio 文档](../vsto/how-to-programmatically-print-visio-documents.md)  
  
  