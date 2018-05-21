---
UID: NN:shobjidl_core.IRegTreeItem
title: IRegTreeItem
author: windows-driver-content
description: Exposes methods that retrieve and set the state of items in a tree-view control that have the Tree-View Control Window Styles flag set.
old-location: shell\IRegTreeItem.htm
old-project: shell
ms.assetid: a9ae0fb3-4a6e-473e-9fa3-d3894834fb72
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IRegTreeItem, IRegTreeItem interface [Windows Shell], IRegTreeItem interface [Windows Shell],described, _win32_IRegTreeItem, shell.IRegTreeItem, shobjidl_core/IRegTreeItem
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
-	Shell32.dll
api_name:
-	IRegTreeItem
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IRegTreeItem interface


## -description


<p class="CCE_Message">[This interface is supported through Windows XP Service Pack 2 (SP2) and Windows Server 2003. It might be unsupported in subsequent versions of Windows.]

Exposes methods that retrieve and set the state of items in a tree-view control that have the <a href="_win32_Tree_View_Control_Window_Styles">Tree-View Control Window Styles</a> flag set.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IRegTreeItem</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IRegTreeItem</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IRegTreeItem</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/bfeff83e-8872-4df2-a519-1335be6e443c">GetCheckState</a>
</td>
<td align="left" width="63%">
Gets the state of a check box item in a tree-view control.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/0ba25491-8d18-4040-a256-9078b91e4f3f">SetCheckState</a>
</td>
<td align="left" width="63%">
Sets the state of a check box item in a tree-view control.

</td>
</tr>
</table> 


## -see-also




<a href="_win32_Tree_View_Controls">Tree-View Controls</a>
 

 
