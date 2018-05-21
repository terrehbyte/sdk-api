---
UID: NF:shobjidl_core.INamespaceWalkCB.EnterFolder
title: INamespaceWalkCB::EnterFolder
author: windows-driver-content
description: Called when a folder is about to be entered during a namespace walk. Use this method for any initialization of the retrieved item.
old-location: shell\INamespaceWalkCB_EnterFolder.htm
old-project: shell
ms.assetid: fd5c25f4-6e48-494b-9d5b-ba1d846ce4d2
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: EnterFolder, EnterFolder method [Windows Shell], EnterFolder method [Windows Shell],INamespaceWalkCB interface, INamespaceWalkCB interface [Windows Shell],EnterFolder method, INamespaceWalkCB.EnterFolder, INamespaceWalkCB::EnterFolder, _win32_INamespaceWalkCB_EnterFolder, shell.INamespaceWalkCB_EnterFolder, shobjidl_core/INamespaceWalkCB::EnterFolder
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
-	INamespaceWalkCB.EnterFolder
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# INamespaceWalkCB::EnterFolder


## -description


Called when a folder is about to be entered during a namespace walk. Use this method for any initialization of the retrieved item.


## -parameters




### -param psf [in]

Type: <b><a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a> object representing the parent of the folder designated by <i>pidl</i>.


### -param pidl [in]

Type: <b>PCUITEMID_CHILD</b>

The PIDL, relative to <i>psf</i>, of the folder being entered.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


