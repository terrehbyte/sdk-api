---
UID: NF:shobjidl_core.IFileOpenDialog.GetSelectedItems
title: IFileOpenDialog::GetSelectedItems
author: windows-driver-content
description: Gets the currently selected items in the dialog. These items may be items selected in the view, or text selected in the file name edit box.
old-location: shell\IFileOpenDialog_GetSelectedItems.htm
old-project: shell
ms.assetid: 5fc53607-60d2-4d23-b11e-779c26c02b0f
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetSelectedItems, GetSelectedItems method [Windows Shell], GetSelectedItems method [Windows Shell],IFileOpenDialog interface, IFileOpenDialog interface [Windows Shell],GetSelectedItems method, IFileOpenDialog.GetSelectedItems, IFileOpenDialog::GetSelectedItems, shell.IFileOpenDialog_GetSelectedItems, shell_IFileOpenDialog_GetSelectedItems, shobjidl_core/IFileOpenDialog::GetSelectedItems
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
-	IFileOpenDialog.GetSelectedItems
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFileOpenDialog::GetSelectedItems


## -description


Gets the currently selected items in the dialog. These items may be items selected in the view, or text selected in the file name edit box.


## -parameters




### -param ppsai [out]

Type: <b><a href="https://msdn.microsoft.com/348213d1-c03f-4c38-9d13-3b1009d94e07">IShellItemArray</a>**</b>

The address of a pointer to an <a href="https://msdn.microsoft.com/348213d1-c03f-4c38-9d13-3b1009d94e07">IShellItemArray</a> through which the selected items can be accessed.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks




              This method can be used for single item or multiple item selections. If the user has entered new text in the file name field, this can be a time-consuming operation. When the application calls this method, the application parses the text in the <code>filename</code> field. For example, if this is a network share, the operation could take some time. However, this operation will not block the UI, since the user should able to stop the operation, which will result in <b>IFileOpenDialog::GetSelectedItems</b> returning a failure code).
            


