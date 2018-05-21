---
UID: NF:shobjidl_core.IPersistIDList.GetIDList
title: IPersistIDList::GetIDList
author: windows-driver-content
description: Gets an item identifier list.
old-location: shell\IPersistIDList_GetIDList.htm
old-project: shell
ms.assetid: 2c05c2f5-5f72-436e-9b71-83749d3217b0
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetIDList, GetIDList method [Windows Shell], GetIDList method [Windows Shell],IPersistIDList interface, IPersistIDList interface [Windows Shell],GetIDList method, IPersistIDList.GetIDList, IPersistIDList::GetIDList, inet_IPersistIDList_GetIDList, shell.IPersistIDList_GetIDList, shobjidl_core/IPersistIDList::GetIDList
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
-	IPersistIDList.GetIDList
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IPersistIDList::GetIDList


## -description


Gets an item identifier list.


## -parameters




### -param ppidl [out]

Type: <b>LPITEMIDLIST*</b>

The address of a pointer to the item identifier list to get.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


