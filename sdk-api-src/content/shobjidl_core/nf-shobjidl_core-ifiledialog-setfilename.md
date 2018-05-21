---
UID: NF:shobjidl_core.IFileDialog.SetFileName
title: IFileDialog::SetFileName
author: windows-driver-content
description: Sets the file name that appears in the File name edit box when that dialog box is opened.
old-location: shell\IFileDialog_SetFileName.htm
old-project: shell
ms.assetid: b8b72a76-6cdb-4675-8d84-f3c7171b8576
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IFileDialog interface [Windows Shell],SetFileName method, IFileDialog.SetFileName, IFileDialog::SetFileName, SetFileName, SetFileName method [Windows Shell], SetFileName method [Windows Shell],IFileDialog interface, _shell_IFileDialog_SetFileName, shell.IFileDialog_SetFileName, shobjidl_core/IFileDialog::SetFileName
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
-	IFileDialog.SetFileName
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileDialog::SetFileName


## -description


Sets the file name that appears in the <b>File name</b> edit box when that dialog box is opened.


## -parameters




### -param pszName [in]

Type: <b>LPCWSTR</b>

A pointer to the name of the file.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


