---
UID: NN:shobjidl_core.IOpenControlPanel
title: IOpenControlPanel
author: windows-driver-content
description: Exposes methods that retrieve the view state of the Control Panel, the path of individual Control Panel items, and that open either the Control Panel itself or an individual Control Panel item.
old-location: shell\IOpenControlPanel.htm
old-project: shell
ms.assetid: fbf86553-7aa1-4a0f-9775-5f71f41b1705
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IOpenControlPanel, IOpenControlPanel interface [Windows Shell], IOpenControlPanel interface [Windows Shell],described, _shell_IOpenControlPanel, shell.IOpenControlPanel, shobjidl_core/IOpenControlPanel
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
-	IOpenControlPanel
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll (version 6.1 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IOpenControlPanel interface


## -description


Exposes methods that retrieve the view state of the Control Panel, the path of individual Control Panel items, and that open either the Control Panel itself or an individual Control Panel item.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOpenControlPanel</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IOpenControlPanel</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IOpenControlPanel</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/ed539638-7953-471f-ac90-ebd4c3929e8e">GetCurrentView</a>
</td>
<td align="left" width="63%">
Gets the most recent Control Panel view: Classic view or Category view.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/mt432961">GetPath</a>
</td>
<td align="left" width="63%">
Gets the path of a specified Control Panel item.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/hh451153">Open</a>
</td>
<td align="left" width="63%">
Opens the specified Control Panel item, optionally to a specific page.

</td>
</tr>
</table> 
