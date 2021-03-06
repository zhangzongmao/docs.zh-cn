---
title: 如何：在 Windows 窗体应用程序中创建 HTML 文档查看器
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- WebBrowser control [Windows Forms], creating an HTML document viewer
- document viewers
- Windows Forms, creating document viewers
ms.assetid: 6a6338fe-f7ee-4f5e-9d8f-0465c57e9039
ms.openlocfilehash: 1330e20cc4fe7df86e51bebca28e4a71e3108673
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-create-an-html-document-viewer-in-a-windows-forms-application"></a>如何：在 Windows 窗体应用程序中创建 HTML 文档查看器
你可以使用<xref:System.Windows.Forms.WebBrowser>控件来显示和打印 HTML 文档，而无需提供 Internet Web 浏览器的完整功能。 当你想要充分利用 HTML 格式设置功能，但不是希望用户可以加载可能包含不受信任的 Web 控件或潜在的恶意脚本代码的任意网页，这非常有用。 你可能想要限制的功能<xref:System.Windows.Forms.WebBrowser>控制这种方式，例如，若要将其用作 HTML 电子邮件查看器，或以 HTML 格式在中提供帮助你的应用程序。  
  
### <a name="to-create-an-html-document-viewer"></a>若要创建 HTML 文档查看器  
  
1.  设置<xref:System.Windows.Forms.WebBrowser.AllowWebBrowserDrop%2A>属性`false`以防止<xref:System.Windows.Forms.WebBrowser>控件打开放到其上的文件。  
  
     [!code-csharp[WebBrowserMisc#20](../../../../samples/snippets/csharp/VS_Snippets_Winforms/WebBrowserMisc/CS/WebBrowserMisc.cs#20)]
     [!code-vb[WebBrowserMisc#20](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/WebBrowserMisc/vb/WebBrowserMisc.vb#20)]  
  
2.  设置<xref:System.Windows.Forms.WebBrowser.Url%2A>属性显示的初始文件的位置。  
  
     [!code-csharp[WebBrowserMisc#21](../../../../samples/snippets/csharp/VS_Snippets_Winforms/WebBrowserMisc/CS/WebBrowserMisc.cs#21)]
     [!code-vb[WebBrowserMisc#21](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/WebBrowserMisc/vb/WebBrowserMisc.vb#21)]  
  
## <a name="compiling-the-code"></a>编译代码  
 此示例需要：  
  
-   名为 `webBrowser1` 的 <xref:System.Windows.Forms.WebBrowser> 控件。  
  
-   对 `System` 和 `System.Windows.Forms` 程序集的引用。  
  
## <a name="see-also"></a>请参阅  
 <xref:System.Windows.Forms.WebBrowser>  
 <xref:System.Windows.Forms.WebBrowser.AllowWebBrowserDrop%2A>  
 <xref:System.Windows.Forms.WebBrowser.Url%2A>  
 [WebBrowser 控件概述](../../../../docs/framework/winforms/controls/webbrowser-control-overview.md)  
 [WebBrowser 安全](../../../../docs/framework/winforms/controls/webbrowser-security.md)  
 [如何：使用 WebBrowser 控件转到 URL](../../../../docs/framework/winforms/controls/how-to-navigate-to-a-url-with-the-webbrowser-control.md)  
 [如何：使用 WebBrowser 控件进行打印](../../../../docs/framework/winforms/controls/how-to-print-with-a-webbrowser-control.md)
