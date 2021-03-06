---
title: 如何：清除自定义控件上的墨迹
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- custom controls [WPF], erasing ink on
- ink [WPF], erasing on custom control
ms.assetid: d88c50f9-b4d8-4962-a28b-67d6a15a5fe0
ms.openlocfilehash: 66c0d19b368b56821fd4034ec4c7cd397b244ab0
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-erase-ink-on-a-custom-control"></a>如何：清除自定义控件上的墨迹
<xref:System.Windows.Ink.IncrementalStrokeHitTester>确定当前绘制的笔画是否与另一个笔画相交。  这是有用的用于创建控件，使用户能够清除笔画部分、 方式用户可以在<xref:System.Windows.Controls.InkCanvas>时<xref:System.Windows.Controls.InkCanvas.EditingMode%2A>设置为<xref:System.Windows.Controls.InkCanvasEditingMode.EraseByPoint>。  
  
## <a name="example"></a>示例  
 下面的示例创建使用户能够清除部分笔画的自定义控件。  此示例创建包含墨迹在初始化的控件。  若要创建收集墨迹的控件，请参阅[创建墨迹输入控件](../../../../docs/framework/wpf/advanced/creating-an-ink-input-control.md)。  
  
 [!code-csharp[HowToEraseInk#1](../../../../samples/snippets/csharp/VS_Snippets_Wpf/HowToEraseInk/CSharp/InkEraser.cs#1)]
 [!code-vb[HowToEraseInk#1](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/HowToEraseInk/VisualBasic/InkEraser.vb#1)]
