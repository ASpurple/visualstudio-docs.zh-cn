---
title: "BoundsRules 约束形状位置和大小 |Microsoft 文档"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
helpviewer_keywords: Domain-Specific Language, events
author: gewarren
ms.author: gewarren
manager: ghogen
ms.workload: multiple
ms.openlocfilehash: 7600f71cc7203b48a6a20da98f59846a0b62bc13
ms.sourcegitcommit: f89ed5fc2e5078213e30a6ade4604e34df48181f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2018
---
# <a name="boundsrules-constrain-shape-location-and-size"></a>BoundsRules 约束形状位置和大小
A*边界规则*是一个类，它定义的大小和形状的位置上的限制。 它提供的用户正在拖动形状或角或两边的形状时重复调用的方法。  
  
 下面的示例约束是条形图的固定大小，水平或垂直矩形形状。 当用户拖动的角或侧时，大纲翻转之间的两个允许的配置的高度和宽度。  
  
 边界规则类派生自<xref:Microsoft.VisualStudio.Modeling.Diagrams.BoundsRules>。 在形状中创建的规则的实例：  
  
```  
using Microsoft.VisualStudio.Modeling.Diagrams; ...  
public partial class BarShape  
{  
  /// <summary>  
  /// Rule invoked when the user is resizing a shape.  
  /// </summary>  
  public override BoundsRules BoundsRules  
  { get { return new BarBoundsRule(); } }  
}  
/// <summary>  
/// Rule invoked when the user is changing a shape's outline.  
/// Provides real-time mouse rubber-band feedback, so must work fast.  
/// </summary>  
public class BarBoundsRule: BoundsRules  
{   
  public override RectangleD GetCompliantBounds   
     (ShapeElement shape, RectangleD proposedBounds)  
  {  
    double thickness = 0.1;  
    if (proposedBounds.Height > proposedBounds.Width)  
    {  
      // There is a minimum width for a shape; the width  
      // will actually be set to the lesser of   
      // thickness and that minimum.  
      return new RectangleD(proposedBounds.Location,   
            new SizeD(thickness, proposedBounds.Height));  
    }  
    else  
    {  
      // There is a minimum height for a shape; the   
      // height will actually be set to the lesser of   
      // thickness and that minimum.  
      return new RectangleD(proposedBounds.Location,   
         new SizeD(proposedBounds.Width, thickness));  
} } }  
```  
  
 请注意是否你想，可以约束的位置和大小。  
  
## <a name="see-also"></a>请参阅  
 <xref:Microsoft.VisualStudio.Modeling.Diagrams.BoundsRules>   
 [响应并传播更改](../modeling/responding-to-and-propagating-changes.md)