---
title: "如何： 以编程方式显示工作表注释 |Microsoft 文档"
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
- worksheets, comments
- comments, worksheets
author: TerryGLee
ms.author: tglee
manager: ghogen
ms.workload: office
ms.openlocfilehash: c43e33030cffc78bc8ee4a0665c9334bc6e8bca7
ms.sourcegitcommit: f9fbf1f55f9ac14e4e5c6ae58c30dc1800ca6cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/10/2018
---
# <a name="how-to-programmatically-display-worksheet-comments"></a>如何：以编程方式显示工作表注释
  可以在 Microsoft Office Excel 工作表中以编程方式显示和隐藏注释。  
  
 [!INCLUDE[appliesto_xlalldocapp](../vsto/includes/appliesto-xlalldocapp-md.md)]  
  
### <a name="to-display-all-comments-on-a-worksheet-in-a-document-level-customization"></a>在文档级自定义项的工作表中显示所有注释  
  
1.  若想显示注释，请将 <xref:Microsoft.Office.Interop.Excel.Comment.Visible%2A> 属性设置为 **true** ；否则为 **false**。 必须将此代码置于表类中，而不是在 `ThisWorkbook` 类中。  
  
     [!code-csharp[Trin_VstcoreExcelAutomation#31](../vsto/codesnippet/CSharp/Trin_VstcoreExcelAutomationCS/Sheet1.cs#31)]
     [!code-vb[Trin_VstcoreExcelAutomation#31](../vsto/codesnippet/VisualBasic/Trin_VstcoreExcelAutomation/Sheet1.vb#31)]  
  
### <a name="to-display-all-comments-on-a-worksheet-in-an-application-level-vsto-add-in"></a>在应用程序级 VSTO 外接程序的工作表中显示所有注释  
  
1.  若想显示注释，请将 <xref:Microsoft.Office.Interop.Excel.Comment.Visible%2A> 属性设置为 **true** ；否则为 **false**。  
  
     [!code-csharp[Trin_VstcoreExcelAutomationAddIn#21](../vsto/codesnippet/CSharp/trin_vstcoreexcelautomationaddin/ThisAddIn.cs#21)]
     [!code-vb[Trin_VstcoreExcelAutomationAddIn#21](../vsto/codesnippet/VisualBasic/trin_vstcoreexcelautomationaddin/ThisAddIn.vb#21)]  
  
## <a name="see-also"></a>请参阅  
 [使用工作表](../vsto/working-with-worksheets.md)   
 [如何： 以编程方式添加和删除工作表注释](../vsto/how-to-programmatically-add-and-delete-worksheet-comments.md)   
 [主机项和主机控件概述](../vsto/host-items-and-host-controls-overview.md)  
  
  