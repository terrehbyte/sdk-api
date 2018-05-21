---
UID: NF:shobjidl_core.IFolderView.GetItemPosition
title: IFolderView::GetItemPosition
author: windows-driver-content
description: Gets the position of an item in the folder's view.
old-location: shell\IFolderView_GetItemPosition.htm
old-project: shell
ms.assetid: 454d074c-1044-4626-8ec7-18e2adb4beca
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetItemPosition, GetItemPosition method [Windows Shell], GetItemPosition method [Windows Shell],IFolderView interface, IFolderView interface [Windows Shell],GetItemPosition method, IFolderView.GetItemPosition, IFolderView::GetItemPosition, _shell_IFolderView_GetItemPosition, shell.IFolderView_GetItemPosition, shobjidl_core/IFolderView::GetItemPosition
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 7 [desktop apps only]
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
-	IFolderView.GetItemPosition
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IFolderView::GetItemPosition


## -description


Gets the position of an item in the folder's view.


## -parameters




### -param pidl [in]

Type: <b>PCUITEMID_CHILD</b>

A pointer to an <a href="https://msdn.microsoft.com/60daf071-4e93-4e1c-bc38-894f706db04f">ITEMIDLIST</a> interface.


### -param ppt [out]

Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/ff569161">POINT</a>*</b>

A pointer to a structure that receives the position of the item's upper-left corner.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


