---
title: 如何：当应用程序启动或关闭时记录消息 (Visual Basic)
ms.date: 07/20/2015
helpviewer_keywords:
- event logs, shutdown
- My.Application.Log object, logging
- Startup event [Visual Basic]
- event logs, startup
- Shutdown event [Visual Basic]
- My.Log object, logging
ms.assetid: 67624d05-cddf-48b7-8c36-5c99baa4c621
ms.openlocfilehash: 80b07e67cb307d461e63df9f94c9d0962eb6374a
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-log-messages-when-the-application-starts-or-shuts-down-visual-basic"></a>如何：当应用程序启动或关闭时记录消息 (Visual Basic)
可以使用 `My.Application.Log` 和 `My.Log` 对象来记录有关应用程序中所发生事件的信息。 本示例将演示如何结合使用 `My.Application.Log.WriteEntry` 方法与 `Startup` 和 `Shutdown` 事件来写入跟踪信息。  
  
### <a name="to-access-the-applications-event-handler-code"></a>访问应用程序的事件处理程序代码  
  
1.  在 **“解决方案资源管理器”** 中选择一个项目。 在 **“项目”** 菜单上，选择 **“属性”**。  
  
2.  单击“应用程序”  选项卡。  
  
3.  单击“查看应用程序事件”  按钮，打开“代码编辑器”。  
  
     此时将打开 ApplicationEvents.vb 文件。  
  
### <a name="to-log-messages-when-the-application-starts"></a>在应用程序启动时记录消息  
  
1.  在“代码编辑器”中打开 ApplicationEvents.vb 文件。 在“常规”  菜单上，选择“MyApplication 事件” 。  
  
2.  在“声明”  菜单上，选择“启动” 。  
  
     在主应用程序运行之前，应用程序将引发 <xref:Microsoft.VisualBasic.ApplicationServices.WindowsFormsApplicationBase.Startup> 事件。  
  
3.  将 `My.Application.Log.WriteEntry` 方法添加到 `Startup` 事件处理程序。  
  
     [!code-vb[VbVbalrMyApplicationLog#1](../../../../visual-basic/developing-apps/programming/log-info/codesnippet/VisualBasic/how-to-log-messages-when-the-application-starts-or-shuts-down_1.vb)]  
  
### <a name="to-log-messages-when-the-application-shuts-down"></a>在应用程序关闭时记录消息  
  
1.  在“代码编辑器”中打开 ApplicationEvents.vb 文件。 在“常规”  菜单上，选择“MyApplication 事件” 。  
  
2.  在“声明”  菜单上，选择“关闭” 。  
  
     在主应用程序运行之后、关闭之前，应用程序将引发 <xref:Microsoft.VisualBasic.ApplicationServices.WindowsFormsApplicationBase.Shutdown> 事件。  
  
3.  将 `My.Application.Log.WriteEntry` 方法添加到 `Shutdown` 事件处理程序。  
  
     [!code-vb[VbVbalrMyApplicationLog#2](../../../../visual-basic/developing-apps/programming/log-info/codesnippet/VisualBasic/how-to-log-messages-when-the-application-starts-or-shuts-down_2.vb)]  
  
## <a name="example"></a>示例  
 可以通过“项目设计器” 访问“代码编辑器”中的应用程序事件。 有关详细信息，请参阅 [Application Page, Project Designer (Visual Basic)](/visualstudio/ide/reference/application-page-project-designer-visual-basic)（应用程序页、项目设计器 (Visual Basic)。  
  
 [!code-vb[VbVbalrMyApplicationLog#3](../../../../visual-basic/developing-apps/programming/log-info/codesnippet/VisualBasic/how-to-log-messages-when-the-application-starts-or-shuts-down_3.vb)]  
  
## <a name="see-also"></a>请参阅  
 <xref:Microsoft.VisualBasic.Logging.Log?displayProperty=nameWithType>  
 <xref:Microsoft.VisualBasic.Logging.Log.WriteEntry%2A>  
 <xref:Microsoft.VisualBasic.Logging.Log.WriteException%2A>  
 [“项目设计器”->“应用程序”页 (Visual Basic)](/visualstudio/ide/reference/application-page-project-designer-visual-basic)  
 [使用应用程序日志](../../../../visual-basic/developing-apps/programming/log-info/working-with-application-logs.md)
