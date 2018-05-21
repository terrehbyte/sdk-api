---
UID: NF:shobjidl_core.ICustomDestinationList.AbortList
title: ICustomDestinationList::AbortList
author: windows-driver-content
description: Discontinues a Jump List building session initiated by ICustomDestinationList::BeginList without committing any changes.
old-location: shell\ICustomDestinationList_AbortList.htm
old-project: shell
ms.assetid: 922eb957-8031-4b4c-9b13-78a86f199bfa
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: AbortList, AbortList method [Windows Shell], AbortList method [Windows Shell],ICustomDestinationList interface, ICustomDestinationList interface [Windows Shell],AbortList method, ICustomDestinationList.AbortList, ICustomDestinationList::AbortList, _shell_ICustomDestinationList_AbortList, shell.ICustomDestinationList_AbortList, shobjidl_core/ICustomDestinationList::AbortList
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
-	ICustomDestinationList.AbortList
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll (version 6.1 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# ICustomDestinationList::AbortList


## -description


Discontinues a Jump List building session initiated by <a href="https://msdn.microsoft.com/431ae6b0-1421-46ec-a06a-38158acb0275">ICustomDestinationList::BeginList</a> without committing any changes.


## -parameters






## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



This method allows an application to use a single <a href="https://msdn.microsoft.com/65a3dab8-3136-416d-bd8a-ca813bfe0533">ICustomDestinationList</a> object for many transactions, because a session can be terminated without committing any new data or destroying the previously stored list.




## -see-also




<a href="https://msdn.microsoft.com/65a3dab8-3136-416d-bd8a-ca813bfe0533">ICustomDestinationList</a>



<a href="https://msdn.microsoft.com/cbf2b07d-d67c-4755-888c-d40692d13cae">Taskbar Extensions</a>
 

 
