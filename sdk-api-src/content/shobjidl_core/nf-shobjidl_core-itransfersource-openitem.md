---
UID: NF:shobjidl_core.ITransferSource.OpenItem
title: ITransferSource::OpenItem
author: windows-driver-content
description: Opens the item for copying. Returns an object that can be enumerated for resources (IShellItemResources).
old-location: shell\ITransferSource_OpenItem.htm
old-project: shell
ms.assetid: 8f051923-2798-43e9-8e8d-95eec5f618aa
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ITransferSource interface [Windows Shell],OpenItem method, ITransferSource.OpenItem, ITransferSource::OpenItem, OpenItem, OpenItem method [Windows Shell], OpenItem method [Windows Shell],ITransferSource interface, _shell_ITransferSource_OpenItem, shell.ITransferSource_OpenItem, shobjidl_core/ITransferSource::OpenItem
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
-	ITransferSource.OpenItem
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ITransferSource::OpenItem


## -description


Opens the item for copying. Returns an object that can be enumerated for resources (<a href="https://msdn.microsoft.com/4ca4a01e-e3c2-46aa-a700-b4b2a1e0112e">IShellItemResources</a>).


## -parameters




### -param psi [in]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

A pointer to the <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> to be opened.


### -param flags




### -param riid [out]

Type: <b>REFIID</b>

A reference to the IID (the interface ID or GUID) of the interface to return in <i>ppv</i>.  This should be an <a href="https://msdn.microsoft.com/4ca4a01e-e3c2-46aa-a700-b4b2a1e0112e">IShellItemResources</a> or an interface derived from <b>IShellItemResources</b>.


### -param ppv [out]

Type: <b>void**</b>

When this method returns, contains the address of a pointer to the interface specified by <i>riid</i>.


#### - dwFlags [in]

Type: <b><a href="https://msdn.microsoft.com/8a3da00a-1d96-444d-acbe-9327620b8d24">TRANSFER_SOURCE_FLAGS</a></b>

The flags that control the file operation. One or more of the <a href="https://msdn.microsoft.com/8a3da00a-1d96-444d-acbe-9327620b8d24">TRANSFER_SOURCE_FLAGS</a> constants.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or one of the following specific Shell codes, or a system error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_YES</b></dt>
</dl>
</td>
<td width="60%">
User responded "Yes" to the dialog.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_USER_RETRY</b></dt>
</dl>
</td>
<td width="60%">
User responded to retry the current action.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_USER_IGNORED</b></dt>
</dl>
</td>
<td width="60%">
User responded "No" to the dialog.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_MERGE</b></dt>
</dl>
</td>
<td width="60%">
User responded to merge folders.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_USER_RETRY_WITH_NEW_NAME</b></dt>
</dl>
</td>
<td width="60%">
User responded to retry the file with new name.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_DONT_PROCESS_CHILDREN</b></dt>
</dl>
</td>
<td width="60%">
Child items should not be processed.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_S_PENDING</b></dt>
</dl>
</td>
<td width="60%">
Error has been queued and will display later.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_E_USER_CANCELLED</b></dt>
</dl>
</td>
<td width="60%">
User canceled the current action.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>COPYENGINE_E_REQUIRES_ELEVATION</b></dt>
</dl>
</td>
<td width="60%">
Operation requires elevated privileges.

</td>
</tr>
</table>
 


