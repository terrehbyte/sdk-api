---
UID: NN:shobjidl_core.IShellIconOverlayIdentifier
title: IShellIconOverlayIdentifier
author: windows-driver-content
description: Exposes methods that handle all communication between icon overlay handlers and the Shell.
old-location: shell\IShellIconOverlayIdentifier.htm
old-project: shell
ms.assetid: c093bc13-def7-411d-b741-50996ffad84b
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IShellIconOverlayIdentifier, IShellIconOverlayIdentifier interface [Windows Shell], IShellIconOverlayIdentifier interface [Windows Shell],described, _win32_IShellIconOverlayIdentifier, shell.IShellIconOverlayIdentifier, shobjidl_core/IShellIconOverlayIdentifier
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: shobjidl_core.h
req.include-header: Shlobj.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
-	Shell32.dll
api_name:
-	IShellIconOverlayIdentifier
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellIconOverlayIdentifier interface


## -description


Exposes methods that handle all communication between icon overlay handlers and the Shell.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IShellIconOverlayIdentifier</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IShellIconOverlayIdentifier</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IShellIconOverlayIdentifier</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/301dc569-738f-454f-9063-223ea6632e55">GetOverlayInfo</a>
</td>
<td align="left" width="63%">
Provides the location of the icon overlay's bitmap.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/c191bcf7-8b49-4276-9e30-2a8dcaf1fc46">GetPriority</a>
</td>
<td align="left" width="63%">
Specifies the priority of an icon overlay.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/02cbe6f3-2ee8-480b-b9c1-a2dbaf80fa26">IsMemberOf</a>
</td>
<td align="left" width="63%">
Specifies whether an icon overlay should be added to a Shell object's icon.

</td>
</tr>
</table> 


## -remarks



Icon overlays are small images placed at the lower-left corner of the icon that represents a Shell object in Windows Explorer or on the desktop. They are used to add some extra information to the object's normal icon. A commonly used icon overlay is the small arrow that indicates that a file or folder is actually a link. You can specify custom icon overlays for Shell objects by implementing and registering an icon overlay handler.

Icon overlay handlers are Component Object Model (COM) objects that are associated with a particular icon overlay. For a general discussion of icon overlay handlers, see <a href="https://msdn.microsoft.com/ADF27BFD-CC96-43F9-9EBB-DEBE0DEA7B92">How to Implement Icon Overlay Handlers</a>.

This interface must be implemented by all icon overlay handlers.

This interface is not typically called by applications.


