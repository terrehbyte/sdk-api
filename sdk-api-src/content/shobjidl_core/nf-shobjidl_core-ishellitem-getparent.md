---
UID: NF:shobjidl_core.IShellItem.GetParent
title: IShellItem::GetParent
author: windows-driver-content
description: Gets the parent of an IShellItem object.
old-location: shell\IShellItem_GetParent.htm
old-project: shell
ms.assetid: d62123af-2ae2-40f2-8581-c95b18491f20
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetParent, GetParent method [Windows Shell], GetParent method [Windows Shell],IShellItem interface, IShellItem interface [Windows Shell],GetParent method, IShellItem.GetParent, IShellItem::GetParent, _win32_IShellItem_GetParent, shell.IShellItem_GetParent, shobjidl_core/IShellItem::GetParent
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
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
-	IShellItem.GetParent
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.00 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellItem::GetParent


## -description


Gets the parent of an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> object.


## -parameters




### -param ppsi

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>**</b>

The address of a pointer to the parent of an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> interface.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or an error value otherwise.




## -see-also




<a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>



<a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>
 

 
