---
UID: NF:shobjidl_core.IEnumObjects.Skip
title: IEnumObjects::Skip
author: windows-driver-content
description: Skips a specified number of objects.
old-location: shell\IEnumObjects_Skip.htm
old-project: shell
ms.assetid: 227be42b-c821-40f4-8bcb-9990d1ceefeb
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IEnumObjects interface [Windows Shell],Skip method, IEnumObjects.Skip, IEnumObjects::Skip, Skip, Skip method [Windows Shell], Skip method [Windows Shell],IEnumObjects interface, _shell_IEnumObjects_Skip, shell.IEnumObjects_Skip, shobjidl_core/IEnumObjects::Skip
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
-	IEnumObjects.Skip
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IEnumObjects::Skip


## -description


Skips a specified number of objects.


## -parameters




### -param celt [in]

Type: <b>ULONG</b>

The number of objects to skip.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Enumeration index is advanced by the number of items skipped.


