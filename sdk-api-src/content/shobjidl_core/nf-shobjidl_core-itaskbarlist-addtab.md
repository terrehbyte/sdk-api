---
UID: NF:shobjidl_core.ITaskbarList.AddTab
title: ITaskbarList::AddTab
author: windows-driver-content
description: Adds an item to the taskbar.
old-location: shell\ITaskbarList_AddTab.htm
old-project: shell
ms.assetid: 47d52ab8-f182-4bfb-8745-ad2d23197088
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: AddTab, AddTab method [Windows Shell], AddTab method [Windows Shell],ITaskbarList interface, ITaskbarList interface [Windows Shell],AddTab method, ITaskbarList.AddTab, ITaskbarList::AddTab, _win32_ITaskbarList_AddTab, shell.ITaskbarList_AddTab, shobjidl_core/ITaskbarList::AddTab
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
-	ITaskbarList.AddTab
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.71 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# ITaskbarList::AddTab


## -description


Adds an item to the taskbar.


## -parameters




### -param hwnd

Type: <b>HWND</b>

A handle to the window to be added to the taskbar.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Any type of window can be added to the taskbar, but it is recommended that the window at least have the <a href="https://msdn.microsoft.com/bfc146f1-bebd-4e68-a29e-a73ff3e8f35b">WS_CAPTION</a> style.

Any window added with this method must be removed with the <a href="https://msdn.microsoft.com/bf1b3d27-5cd3-44c8-81e6-d9418d30ffe3">DeleteTab</a> method when the added window is destroyed.


