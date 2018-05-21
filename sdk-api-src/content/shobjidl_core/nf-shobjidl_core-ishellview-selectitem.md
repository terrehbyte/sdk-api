---
UID: NF:shobjidl_core.IShellView.SelectItem
title: IShellView::SelectItem
author: windows-driver-content
description: Changes the selection state of one or more items within the Shell view window.
old-location: shell\IShellView_SelectItem.htm
old-project: shell
ms.assetid: 5c34c05e-175c-43cb-9fbb-2eb3e2b39f6f
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IShellView interface [Windows Shell],SelectItem method, IShellView.SelectItem, IShellView::SelectItem, SelectItem, SelectItem method [Windows Shell], SelectItem method [Windows Shell],IShellView interface, _win32_IShellView_SelectItem, shell.IShellView_SelectItem, shobjidl_core/IShellView::SelectItem
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
-	IShellView.SelectItem
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellView::SelectItem


## -description


Changes the selection state of one or more items within the Shell view window.


## -parameters




### -param pidlItem

Type: <b>PCUITEMID_CHILD</b>

The address of the <a href="https://msdn.microsoft.com/60daf071-4e93-4e1c-bc38-894f706db04f">ITEMIDLIST</a> structure.


### -param uFlags

Type: <b>UINT</b>

One of the <a href="https://msdn.microsoft.com/3b0a7ec3-f365-48ec-86b0-ffd4c345deaf">_SVSIF</a> constants that specify the type of selection to apply.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<h3><a id="Notes_to_Implementers"></a><a id="notes_to_implementers"></a><a id="NOTES_TO_IMPLEMENTERS"></a>Notes to Implementers</h3>
This method is used to implement the Target command from the <b>File</b> menu of the Shell shortcut property sheet.




## -see-also




<a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a>
 

 
