---
UID: NF:shobjidl_core.IFileDialog.GetFolder
title: IFileDialog::GetFolder
author: windows-driver-content
description: Gets either the folder currently selected in the dialog, or, if the dialog is not currently displayed, the folder that is to be selected when the dialog is opened.
old-location: shell\IFileDialog_GetFolder.htm
old-project: shell
ms.assetid: 424d1507-e42a-43d7-8904-347bfb311dd4
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetFolder, GetFolder method [Windows Shell], GetFolder method [Windows Shell],IFileDialog interface, IFileDialog interface [Windows Shell],GetFolder method, IFileDialog.GetFolder, IFileDialog::GetFolder, shell.IFileDialog_GetFolder, shell_IFileDialog_GetFolder, shobjidl_core/IFileDialog::GetFolder
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
-	IFileDialog.GetFolder
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileDialog::GetFolder


## -description


Gets either the folder currently selected in the dialog, or, if the dialog is not currently displayed, the folder that is to be selected when the dialog is opened.


## -parameters




### -param ppsi [out]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>**</b>

The address of a pointer to the interface that represents the folder.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The calling application is responsible for releasing the retrieved <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> when it is no longer needed.


