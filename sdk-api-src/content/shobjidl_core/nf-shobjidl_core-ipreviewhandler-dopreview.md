---
UID: NF:shobjidl_core.IPreviewHandler.DoPreview
title: IPreviewHandler::DoPreview
author: windows-driver-content
description: Directs the preview handler to load data from the source specified in an earlier Initialize method call, and to begin rendering to the previewer window.
old-location: shell\IPreviewHandler_DoPreview.htm
old-project: shell
ms.assetid: f6bad84f-9089-4905-ad4d-9b69ff9d11d6
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: DoPreview, DoPreview method [Windows Shell], DoPreview method [Windows Shell],IPreviewHandler interface, IPreviewHandler interface [Windows Shell],DoPreview method, IPreviewHandler.DoPreview, IPreviewHandler::DoPreview, _shell_IPreviewHandler_DoPreview, shell.IPreviewHandler_DoPreview, shobjidl_core/IPreviewHandler::DoPreview
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	shobjidl_core.h
api_name:
-	IPreviewHandler.DoPreview
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IPreviewHandler::DoPreview


## -description


Directs the preview handler to load data from the source specified in an earlier Initialize method call, and to begin rendering to the previewer window.


## -parameters






## -returns



Type: <b>HRESULT</b>

This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The operation completed successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_PREVIEWHANDLER_DRM_FAIL</b></dt>
</dl>
</td>
<td width="60%">
Blocked by digital rights management.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_PREVIEWHANDLER_NOAUTH</b></dt>
</dl>
</td>
<td width="60%">
Blocked by file permissions.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_PREVIEWHANDLER_NOTFOUND</b></dt>
</dl>
</td>
<td width="60%">
Item was not found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_PREVIEWHANDLER_CORRUPT</b></dt>
</dl>
</td>
<td width="60%">
Item was corrupt.

</td>
</tr>
</table>
 




## -remarks



If the previewer window has not yet been created, then it must be created after this method has been called. The preview handler is responsible for painting the area specified in <a href="https://msdn.microsoft.com/a323811a-8244-40a0-a6b2-68572639be5f">IPreviewHandler::SetWindow</a> or <a href="https://msdn.microsoft.com/03353962-6905-4b13-bf7a-f1767767a7df">IPreviewHandler::SetRect</a>.  If these methods are called while the preview handler is rendering, the window must be reparented/resized without stopping or restarting the rendering of the item.

This method should be called only after <a href="https://msdn.microsoft.com/a323811a-8244-40a0-a6b2-68572639be5f">IPreviewHandler::SetWindow</a> has been called.


              Aditionally, this method should be called only after <a href="https://msdn.microsoft.com/library/windows/hardware/ff550945">Initialize</a>, <a href="https://msdn.microsoft.com/library/windows/hardware/ff550945">Initialize</a>, or <a href="https://msdn.microsoft.com/library/windows/hardware/ff550945">Initialize</a> has been called.
            

<div class="alert"><b>Note</b>  Do not actually create the previewer window until this method has been called.</div>
<div> </div>

