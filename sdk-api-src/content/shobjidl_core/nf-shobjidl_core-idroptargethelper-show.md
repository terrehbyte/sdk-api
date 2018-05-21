---
UID: NF:shobjidl_core.IDropTargetHelper.Show
title: IDropTargetHelper::Show
author: windows-driver-content
description: Notifies the drag-image manager to show or hide the drag image.
old-location: shell\IDropTargetHelper_Show.htm
old-project: shell
ms.assetid: 412a87d6-4915-4791-b109-060cc967dbc9
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IDropTargetHelper interface [Windows Shell],Show method, IDropTargetHelper.Show, IDropTargetHelper::Show, Show, Show method [Windows Shell], Show method [Windows Shell],IDropTargetHelper interface, _win32_IDropTargetHelper_Show, shell.IDropTargetHelper_Show, shobjidl_core/IDropTargetHelper::Show
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
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
-	Shell32.dll
api_name:
-	IDropTargetHelper.Show
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IDropTargetHelper::Show


## -description


Notifies the drag-image manager to show or hide the drag image.


## -parameters




### -param fShow [in]

Type: <b>BOOL</b>

A boolean value that is set to <b>TRUE</b> to show the drag image, and <b>FALSE</b> to hide it.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or a COM error value otherwise.




## -remarks



This method is used when dragging over a target window in a low color-depth video mode. It allows the target to notify the drag-image manager to hide the drag image while it is painting the window. While you are painting a window that is currently being dragged over, hide the drag image by calling <b>Show</b> with <i>fShow</i> set to <b>FALSE</b>. Once the window has been painted, display the drag image again by calling <b>Show</b> with <i>fShow</i> set to <b>TRUE</b>.




## -see-also




<a href="https://msdn.microsoft.com/b1ddbf7e-edf3-48fb-8983-ae39cb7bb4b0">IDropTargetHelper</a>
 

 
