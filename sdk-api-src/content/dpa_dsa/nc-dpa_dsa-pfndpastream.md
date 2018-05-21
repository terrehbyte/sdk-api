---
UID: NC:dpa_dsa.PFNDPASTREAM
title: PFNDPASTREAM
author: windows-driver-content
description: Defines the prototype for the callback function used by DPA_LoadStream and DPA_SaveStream.
old-location: controls\PFNDPASTREAM.htm
old-project: Controls
ms.assetid: VS|Controls|~\controls\common\functions\pfndpastream.htm
ms.author: windowsdriverdev
ms.date: 5/17/2018
ms.keywords: PFNDPASTREAM, PFNDPASTREAM callback, PFNDPASTREAM callback function [Windows Controls], _win32_PFNDPASTREAM_Function, _win32_PFNDPASTREAM_Function_cpp, controls.PFNDPASTREAM, controls._win32_PFNDPASTREAM_Function, dpa_dsa/PFNDPASTREAM
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: dpa_dsa.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: CRYPTPROTECT_PROMPTSTRUCT, *PCRYPTPROTECT_PROMPTSTRUCT
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	dpa_dsa.h
api_name:
-	PFNDPASTREAM
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# PFNDPASTREAM callback function


## -description


Defines the prototype for the callback function used by <a href="https://msdn.microsoft.com/c06e0851-1a05-4f5e-9ace-53ca220c54ee">DPA_LoadStream</a> and <a href="https://msdn.microsoft.com/96c6649d-c343-4cbd-a4ec-3eef6c52023f">DPA_SaveStream</a>.


## -parameters




### -param *pinfo [in]

Type: <b>DPASTREAMINFO*</b>

A pointer to a <a href="https://msdn.microsoft.com/bd2efbba-2b63-4121-92fd-181d16f300d9">DPASTREAMINFO</a> structure.


### -param *pstream [in]

Type: <b>struct IStream*</b>

An <a href="https://msdn.microsoft.com/c6f60e37-eadc-46a1-94f6-cacc23613531">IStream</a> object to read from or write to.


### -param *pvInstData [in, optional]

Type: <b>void*</b>

A void pointer to callback data that the client passed to <a href="https://msdn.microsoft.com/c06e0851-1a05-4f5e-9ace-53ca220c54ee">DPA_LoadStream</a> or <a href="https://msdn.microsoft.com/96c6649d-c343-4cbd-a4ec-3eef6c52023f">DPA_SaveStream</a>.


## -returns



Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HRESULT</a></b>

If this callback function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


