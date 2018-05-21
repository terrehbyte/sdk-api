---
UID: NF:shobjidl_core.INameSpaceTreeControl.GetItemRect
title: INameSpaceTreeControl::GetItemRect
author: windows-driver-content
description: Gets the RECT structure that describes the size and position of a given item.
old-location: shell\INameSpaceTreeControl_GetItemRect.htm
old-project: shell
ms.assetid: 57e7707c-0fe2-4cde-87d8-2d58e7c06bba
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetItemRect, GetItemRect method [Windows Shell], GetItemRect method [Windows Shell],INameSpaceTreeControl interface, INameSpaceTreeControl interface [Windows Shell],GetItemRect method, INameSpaceTreeControl.GetItemRect, INameSpaceTreeControl::GetItemRect, _shell_INameSpaceTreeControl_GetItemRect, shell.INameSpaceTreeControl_GetItemRect, shobjidl_core/INameSpaceTreeControl::GetItemRect
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
-	INameSpaceTreeControl.GetItemRect
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# INameSpaceTreeControl::GetItemRect


## -description


Gets the <a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a> structure that describes the size and position of a given item.


## -parameters




### -param psi [in]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

A pointer to the item for which the <a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a> structure is being retrieved.


### -param prect [out]

Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a>*</b>

A pointer to the <a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a> structure that describes the size and position of the item.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


