---
UID: NF:shobjidl_core.ITransferDestination.CreateItem
title: ITransferDestination::CreateItem
author: windows-driver-content
description: Creates the specified file.
old-location: shell\ITransferDestination_CreateItem.htm
old-project: shell
ms.assetid: 56a02dd1-2118-4585-b6e9-8223c086b48a
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: CreateItem, CreateItem method [Windows Shell], CreateItem method [Windows Shell],ITransferDestination interface, ITransferDestination interface [Windows Shell],CreateItem method, ITransferDestination.CreateItem, ITransferDestination::CreateItem, _shell_ITransferDestination_CreateItem, shell.ITransferDestination_CreateItem, shobjidl_core/ITransferDestination::CreateItem
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
-	ITransferDestination.CreateItem
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ITransferDestination::CreateItem


## -description


Creates the specified file.


## -parameters




### -param pszName [in]

Type: <b>LPCWSTR</b>

A pointer to a null-terminated buffer that contains the name of the file relative to the current directory.


### -param dwAttributes [in]

Type: <b>DWORD</b>

One or more of the FILE_ATTRIBUTE flags defined in the <a href="https://msdn.microsoft.com/a6fc5cf0-d3b0-4a76-af8b-6a13ab32157d">BY_HANDLE_FILE_INFORMATION</a> structure. The most significant value is FILE_ATTRIBUTE_DIRECTORY, which indicates that a folder should be created.


### -param ullSize [in]

Type: <b>ULONGLONG</b>

The size, in bytes, of the file to create. This value can be 0 if the size is unknown.


### -param flags [in]

Type: <b><a href="https://msdn.microsoft.com/8a3da00a-1d96-444d-acbe-9327620b8d24">TRANSFER_SOURCE_FLAGS</a></b>

Flags that control the file operation. One or more of the <a href="https://msdn.microsoft.com/8a3da00a-1d96-444d-acbe-9327620b8d24">TRANSFER_SOURCE_FLAGS</a> flags.


### -param riidItem [out]

Type: <b>REFIID</b>

A reference to the IID of the interface to retrieve through <i>ppvItem</i>, typically IID_IShellItem or another interface that derives from it.


### -param ppvItem [out]

Type: <b>void**</b>

When this method returns, contains the interface pointer requested in <i>riidItem</i>. This is typically <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> or a derived interface.


### -param riidResources [in]

Type: <b>REFIID</b>

A reference to the IID of the interface to retrieve through <i>ppvResources</i>, typically IID_IShellItemResources or another interface that derives from it.


### -param ppvResources [out]

Type: <b>void**</b>

When this method returns, contains the interface pointer requested in <i>riidResources</i>. This is typically <a href="https://msdn.microsoft.com/4ca4a01e-e3c2-46aa-a700-b4b2a1e0112e">IShellItemResources</a> or a derived interface.


## -returns



Type: <b>HRESULT</b>

Returns a success code if successful, or an error value otherwise. Success codes include:
                
                    

<ul>
<li><b>S_OK</b>: The move succeeded and <i>ppvItem</i> and <i>ppvResources</i> both point to valid objects.</li>
<li><b>COPYENGINE_S_USER_IGNORED</b>: The destination item already exists and has not been overwritten. The values pointed to by <i>ppvItem</i> and <i>ppvResources</i> are <b>NULL</b>. If the caller is implementing a move as a copy and delete operation, the caller should complete the move by deleting the source item.</li>
</ul>



## -remarks



This method may be used to create a Shell item object representing the destination folder for a copy or move operation. The <a href="https://msdn.microsoft.com/341966d4-f9cf-457d-97ef-8e6107544283">ITransferSource</a> interface provides methods to actually move objects of <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> to the destination.

Call <a href="https://msdn.microsoft.com/e25040dd-bb51-45cc-99fb-9113e26d0baa">ITransferDestination::Advise</a> before calling any other <a href="https://msdn.microsoft.com/8d0049e0-e227-40ae-a282-cdc17f227e24">ITransferDestination</a> methods so the handler can callback on any errors that might occur. If not set, the handler should consider it an indication that no feedback is available and to do the "default" operation.

It is recommended that you use the <b>IID_PPV_ARGS</b> macro, defined in Objbase.h, to package the <i>riidResources</i> and <i>ppvResources</i> parameters. This macro provides the correct IID based on the interface pointed to by the value in <i>ppvResources</i>, which eliminates the possibility of a coding error.


