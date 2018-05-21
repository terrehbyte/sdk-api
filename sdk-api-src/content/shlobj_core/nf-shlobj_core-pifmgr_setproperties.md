---
UID: NF:shlobj_core.PifMgr_SetProperties
title: PifMgr_SetProperties function
author: windows-driver-content
description: Assigns values to a block of data from a .pif file.
old-location: properties\PifMgr_SetProperties.htm
old-project: properties
ms.assetid: 720ed580-1867-4651-aef6-24ac4397ad39
ms.author: windowsdriverdev
ms.date: 5/8/2018
ms.keywords: PifMgr_SetProperties, PifMgr_SetProperties function [Windows Properties], _win32_PifMgr_SetProperties, properties.PifMgr_SetProperties, shell.PifMgr_SetProperties, shlobj_core/PifMgr_SetProperties
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: shlobj_core.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: AUTOCOMPLETELISTOPTIONS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Shell32.dll
api_name:
-	PifMgr_SetProperties
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Internet Explorer 5.0
---

# PifMgr_SetProperties function


## -description


<p class="CCE_Message">[<b>PifMgr_SetProperties</b> is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.]

Assigns values to a block of data from a .pif file.


## -parameters




### -param hProps [in, optional]

Type: <b>HANDLE</b>

A handle to the application's properties. This parameter should be set to the value that is returned by <a href="https://msdn.microsoft.com/0bc11528-7278-4765-b3cb-671ba82c9155">PifMgr_OpenProperties</a>.


### -param pszGroup [in, optional]

Type: <b>PCSTR</b>

A null-terminated ANSI string containing the property group name. It can be one of the following, or any other name that corresponds to a valid .pif extension.



#### 

"WINDOWS 286 3.0"

"WINDOWS 386 3.0"

"WINDOWS VMM 4.0"

"WINDOWS NT  3.1"

"WINDOWS NT  4.0"


### -param lpProps [in]

Type: <b>const void*</b>

A property group record buffer that holds the data.


### -param cbProps

Type: <b>int</b>

The size of the buffer, in bytes, pointed to by <i>lpProps</i>.


### -param flOpt

Type: <b>UINT</b>

Always SETPROPS_NONE.


## -returns



Type: <b>int</b>

Returns the amount of information transferred, in bytes. Returns zero if the group cannot be found or an error occurs.




## -see-also




<a href="https://msdn.microsoft.com/62933ddf-9b0d-427a-8b5f-a0117a3b4885">PifMgr_GetProperties</a>
 

 
