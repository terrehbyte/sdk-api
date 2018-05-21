---
UID: NF:shobjidl_core.SHShowManageLibraryUI
title: SHShowManageLibraryUI function
author: windows-driver-content
description: Shows the library management dialog box, which enables users to manage the library folders and default save location.
old-location: shell\SHShowManageLibraryUI.htm
old-project: shell
ms.assetid: 1ac911bb-28d6-4cb6-a66a-1a0c8a4bd6a1
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: SHShowManageLibraryUI, SHShowManageLibraryUI function [Windows Shell], _shell_SHShowManageLibraryUI, shell.SHShowManageLibraryUI, shobjidl_core/SHShowManageLibraryUI
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Shell32.dll
api_name:
-	SHShowManageLibraryUI
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# SHShowManageLibraryUI function


## -description


Shows the library management dialog box, which enables users to manage the library folders and default save location.


## -parameters




### -param psiLibrary [in]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

A pointer to an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> object that represents the library that is to be managed.


### -param hwndOwner [in, optional]

Type: <b>HWND</b>

The handle for the window that owns the library management dialog box. The value of this parameter can be <b>NULL</b>.


### -param pszTitle [in, optional]

Type: <b>LPCWSTR</b>

A pointer to the title for the library management dialog. To display the generic title string, set the value of this parameter to <b>NULL</b>.


### -param pszInstruction [in, optional]

Type: <b>LPCWSTR</b>

A pointer to a help string to display below the title string in the library management dialog box. To display the generic help string, set the value of this parameter to <b>NULL</b>.


### -param lmdOptions [in]

Type: <b><a href="https://msdn.microsoft.com/e5eaf131-9562-4ab0-a8bc-4eaaaa806a8f">LIBRARYMANAGEDIALOGOPTIONS</a></b>

A value from the <a href="https://msdn.microsoft.com/e5eaf131-9562-4ab0-a8bc-4eaaaa806a8f">LIBRARYMANAGEDIALOGOPTIONS</a> enumeration that specifies the behavior of the management dialog box.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/c1ef3d22-7c88-42b0-93a2-5d1b75c327ba">IShellLibrary</a>



<a href="https://msdn.microsoft.com/e5eaf131-9562-4ab0-a8bc-4eaaaa806a8f">LIBRARYMANAGEDIALOGOPTIONS</a>
 

 
