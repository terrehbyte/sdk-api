---
UID: NF:shobjidl_core.IActionProgressDialog.Initialize
title: IActionProgressDialog::Initialize
author: windows-driver-content
description: Provides details about the action progress dialog.
old-location: shell\IActionProgressDialog_Initialize.htm
old-project: shell
ms.assetid: e82f4686-75c6-4f06-8468-937352fe33d3
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IActionProgressDialog interface [Windows Shell],Initialize method, IActionProgressDialog.Initialize, IActionProgressDialog::Initialize, Initialize, Initialize method [Windows Shell], Initialize method [Windows Shell],IActionProgressDialog interface, SPINITF_MODAL, SPINITF_NOMINIMIZE, SPINITF_NORMAL, _shell_IActionProgressDialog_Initialize, shell.IActionProgressDialog_Initialize, shobjidl_core/IActionProgressDialog::Initialize
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
-	Browseui.dll
api_name:
-	IActionProgressDialog.Initialize
product: Windows
targetos: Windows
req.lib: 
req.dll: Browseui.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IActionProgressDialog::Initialize


## -description


Provides details about the action progress dialog.


## -parameters




### -param flags [in]

Type: <b>SPINITF</b>

One of the following values.



#### SPINITF_NORMAL (0x01)

Use the default progress dialog behavior.



#### SPINITF_MODAL (0x01)

Use a modal window for the dialog.



#### SPINITF_NOMINIMIZE (0x08)

Do not display a minimize button.


### -param pszTitle [in]

Type: <b>LPCWSTR</b>

The title of the progress dialog.


### -param pszCancel [in]

Type: <b>LPCWSTR</b>

The string displayed when a user closes the dialog before completion.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


