---
UID: NF:shobjidl_core.IShellBrowser.OnViewWindowActive
title: IShellBrowser::OnViewWindowActive
author: windows-driver-content
description: Called by the Shell view when the view window or one of its child windows gets the focus or becomes active.
old-location: shell\IShellBrowser_OnViewWindowActive.htm
old-project: shell
ms.assetid: bd320262-f383-453b-9028-4e93f0b3761a
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IShellBrowser interface [Windows Shell],OnViewWindowActive method, IShellBrowser.OnViewWindowActive, IShellBrowser::OnViewWindowActive, OnViewWindowActive, OnViewWindowActive method [Windows Shell], OnViewWindowActive method [Windows Shell],IShellBrowser interface, _win32_IShellBrowser_OnViewWindowActive, shell.IShellBrowser_OnViewWindowActive, shobjidl_core/IShellBrowser::OnViewWindowActive
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
-	IShellBrowser.OnViewWindowActive
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellBrowser::OnViewWindowActive


## -description


Called by the Shell view when the view window or one of its child windows gets the focus or becomes active.


## -parameters




### -param pshv






#### - ppshv

Type: <b><a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a>*</b>

Address of the view object's <a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a> pointer.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or a COM-defined error value otherwise.




## -remarks



The view must pass its <a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a> implementation to this routine, although the current version of Windows Explorer does not use this parameter.

<h3><a id="Notes_to_Callers"></a><a id="notes_to_callers"></a><a id="NOTES_TO_CALLERS"></a>Notes to Callers</h3>
The Shell view object must call this method before calling the <a href="https://msdn.microsoft.com/62cbb593-7459-4a4f-96a2-3ec2287e6a26">IShellBrowser::InsertMenusSB</a> method. This method will insert a different set of menu items depending on whether the view has the focus.

<h3><a id="Notes_to_Implementers"></a><a id="notes_to_implementers"></a><a id="NOTES_TO_IMPLEMENTERS"></a>Notes to Implementers</h3>
This method informs the browser that the view is getting the focus (when the mouse is clicked on the view, for example).




## -see-also




<a href="https://msdn.microsoft.com/138d90e3-a1f0-4faf-88ca-16c7a46df0ca">IShellBrowser</a>
 

 
