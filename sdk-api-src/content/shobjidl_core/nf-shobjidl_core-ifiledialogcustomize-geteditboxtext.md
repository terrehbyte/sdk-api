---
UID: NF:shobjidl_core.IFileDialogCustomize.GetEditBoxText
title: IFileDialogCustomize::GetEditBoxText
author: windows-driver-content
description: Gets the current text in an edit box control.
old-location: shell\IFileDialogCustomize_GetEditBoxText.htm
old-project: shell
ms.assetid: 7c3db511-d357-48b4-9ac3-07f6b3d23a5f
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetEditBoxText, GetEditBoxText method [Windows Shell], GetEditBoxText method [Windows Shell],IFileDialogCustomize interface, IFileDialogCustomize interface [Windows Shell],GetEditBoxText method, IFileDialogCustomize.GetEditBoxText, IFileDialogCustomize::GetEditBoxText, shell.IFileDialogCustomize_GetEditBoxText, shell_IFileDialogCustomize_GetEditBoxText, shobjidl_core/IFileDialogCustomize::GetEditBoxText
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
-	IFileDialogCustomize.GetEditBoxText
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileDialogCustomize::GetEditBoxText


## -description


Gets the current text in an edit box control.


## -parameters




### -param dwIDCtl [in]

Type: <b>DWORD</b>

The ID of the edit box.


### -param ppszText [out]

Type: <b>WCHAR**</b>

The address of a pointer to a buffer that receives the text as a null-terminated Unicode string.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



It is the responsibility of the calling application to free the buffer referenced by <i>ppszText</i> when it is no longer needed. Use <a href="https://msdn.microsoft.com/3d0af12e-fc74-4ef7-b2dd-e9da5d0483c7">CoTaskMemFree</a> to free the buffer.


