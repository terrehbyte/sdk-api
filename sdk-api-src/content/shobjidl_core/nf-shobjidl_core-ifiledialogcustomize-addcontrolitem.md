---
UID: NF:shobjidl_core.IFileDialogCustomize.AddControlItem
title: IFileDialogCustomize::AddControlItem
author: windows-driver-content
description: Adds an item to a container control in the dialog.
old-location: shell\IFileDialogCustomize_AddControlItem.htm
old-project: shell
ms.assetid: 56d7d0df-0c3e-4bc3-b91e-3b191f5dad76
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: AddControlItem, AddControlItem method [Windows Shell], AddControlItem method [Windows Shell],IFileDialogCustomize interface, IFileDialogCustomize interface [Windows Shell],AddControlItem method, IFileDialogCustomize.AddControlItem, IFileDialogCustomize::AddControlItem, shell.IFileDialogCustomize_AddControlItem, shell_IFileDialogCustomize_AddControlItem, shobjidl_core/IFileDialogCustomize::AddControlItem
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
-	IFileDialogCustomize.AddControlItem
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileDialogCustomize::AddControlItem


## -description


Adds an item to a container control in the dialog.


## -parameters




### -param dwIDCtl [in]

Type: <b>DWORD</b>

 The ID of the container control to which the item is to be added.


### -param dwIDItem [in]

Type: <b>DWORD</b>

The ID of the item.


### -param pszLabel [in]

Type: <b>LPCWSTR</b>

A pointer to a buffer that contains the item's text, which can be either a label or, in the case of a drop-down list, the item itself. This text is a null-terminated Unicode string.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The default state for this item is enabled and visible. Items in control groups cannot be changed after they have been created, with the exception of their enabled and visible states.

Container controls include option button groups, combo boxes, drop-down lists on the <b>Open</b> or <b>Save</b> button, and menus.


