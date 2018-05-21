---
UID: NF:shobjidl_core.IFolderView2.GetSortColumnCount
title: IFolderView2::GetSortColumnCount
author: windows-driver-content
description: Gets the count of sort columns currently applied to the view.
old-location: shell\IFolderView2_GetSortColumnCount.htm
old-project: shell
ms.assetid: 26590565-f992-4f14-bbbc-4099a1a3ac11
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetSortColumnCount, GetSortColumnCount method [Windows Shell], GetSortColumnCount method [Windows Shell],IFolderView2 interface, IFolderView2 interface [Windows Shell],GetSortColumnCount method, IFolderView2.GetSortColumnCount, IFolderView2::GetSortColumnCount, _shell_IFolderView2_GetSortColumnCount, shell.IFolderView2_GetSortColumnCount, shobjidl_core/IFolderView2::GetSortColumnCount
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
-	IFolderView2.GetSortColumnCount
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFolderView2::GetSortColumnCount


## -description


Gets the count of sort columns currently applied to the view.


## -parameters




### -param pcColumns [out]

Type: <b>int*</b>

A pointer to an <b>int</b>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Returns E_INVALIDARG if the column count provided does not equal the count of sort columns in the view.


