---
UID: NF:shobjidl_core.IParentAndItem.GetParentAndItem
title: IParentAndItem::GetParentAndItem
author: windows-driver-content
description: Gets the parent of an item and the parent's child ID.
old-location: shell\IParentAndItem_GetParentAndItem.htm
old-project: shell
ms.assetid: 351ad043-949c-46e1-a6cd-bcc15016f42a
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetParentAndItem, GetParentAndItem method [Windows Shell], GetParentAndItem method [Windows Shell],IParentAndItem interface, IParentAndItem interface [Windows Shell],GetParentAndItem method, IParentAndItem.GetParentAndItem, IParentAndItem::GetParentAndItem, _shell_IParentAndItem_GetParentAndItem, shell.IParentAndItem_GetParentAndItem, shobjidl_core/IParentAndItem::GetParentAndItem
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
-	IParentAndItem.GetParentAndItem
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IParentAndItem::GetParentAndItem


## -description


Gets the parent of an item and the parent's child ID.


## -parameters




### -param ppidlParent [out, optional]

Type: <b>PIDLIST_ABSOLUTE*</b>

When this method returns, contains the address of a PIDL that specifies the parent.


### -param ppsf [out, optional]

Type: <b><a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>**</b>

When this method returns, contains the address of a pointer to the <a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a> that is the parent.


### -param ppidlChild [out, optional]

Type: <b>PITEMID_CHILD*</b>

When this method returns, contains the address of a child PIDL that identifies the <a href="https://msdn.microsoft.com/5cca426f-73fb-4b39-8eb0-16c01673c311">IParentAndItem</a> object relative to that specified by <i>ppsf</i>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



 While <a href="https://msdn.microsoft.com/5cca426f-73fb-4b39-8eb0-16c01673c311">IParentAndItem</a> is typically implemented on IShellItems, it is not specific to <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>.


