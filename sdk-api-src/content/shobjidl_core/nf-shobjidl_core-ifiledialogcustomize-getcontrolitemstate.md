---
UID: NF:shobjidl_core.IFileDialogCustomize.GetControlItemState
title: IFileDialogCustomize::GetControlItemState
author: windows-driver-content
description: Gets the current state of an item in a container control found in the dialog.
old-location: shell\IFileDialogCustomize_GetControlItemState.htm
old-project: shell
ms.assetid: 62fc28c4-3e6d-4141-b5c7-e7659a1a15c2
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetControlItemState, GetControlItemState method [Windows Shell], GetControlItemState method [Windows Shell],IFileDialogCustomize interface, IFileDialogCustomize interface [Windows Shell],GetControlItemState method, IFileDialogCustomize.GetControlItemState, IFileDialogCustomize::GetControlItemState, shell.IFileDialogCustomize_GetControlItemState, shell_IFileDialogCustomize_GetControlItemState, shobjidl_core/IFileDialogCustomize::GetControlItemState
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
-	IFileDialogCustomize.GetControlItemState
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileDialogCustomize::GetControlItemState


## -description


Gets the current state of an item in a container control found in the dialog.


## -parameters




### -param dwIDCtl [in]

Type: <b>DWORD</b>

The ID of the container control.


### -param dwIDItem [in]

Type: <b>DWORD</b>

The ID of the item.


### -param pdwState [out]

Type: <b>CDCONTROLSTATEF*</b>

A pointer to a variable that receives one of more values from the <a href="https://msdn.microsoft.com/5e556aa2-2e1b-4f71-b386-328405f4aae0">CDCONTROLSTATE</a> enumeration that indicate the current state of the control.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The default state of a control item is enabled and visible. Items in control groups cannot be changed after they have been created, with the exception of their enabled and visible states.

Container controls include option button groups, combo boxes, drop-down lists on the <b>Open</b> or <b>Save</b> button, and menus.


