---
UID: NF:shobjidl_core.IShellItem2.GetUInt64
title: IShellItem2::GetUInt64
author: windows-driver-content
description: Gets the UInt64 value of a specified property key.
old-location: shell\IShellItem2_GetUInt64.htm
old-project: shell
ms.assetid: 3c8a180f-336f-4887-b04b-dbe8f34d4302
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetUInt64, GetUInt64 method [Windows Shell], GetUInt64 method [Windows Shell],IShellItem2 interface, IShellItem2 interface [Windows Shell],GetUInt64 method, IShellItem2.GetUInt64, IShellItem2::GetUInt64, _shell_IShellItem2_GetUInt64, shell.IShellItem2_GetUInt64, shobjidl_core/IShellItem2::GetUInt64
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
-	IShellItem2.GetUInt64
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IShellItem2::GetUInt64


## -description


Gets the UInt64 value of a specified property key.


## -parameters




### -param key [in]

Type: <b>REFPROPERTYKEY</b>

A reference to a <a href="https://msdn.microsoft.com/3f5f31af-f040-443b-9045-9761055381ea">PROPERTYKEY</a> structure.


### -param pull [out]

Type: <b>ULONGLONG*</b>

A pointer to a UInt64 value.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


