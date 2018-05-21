---
UID: NF:oaidl.VARIANT_UserMarshal64
title: VARIANT_UserMarshal64 function
author: windows-driver-content
description: Marshals a VARIANT object into the RPC buffer.
old-location: automat\variant_usermarshal64.htm
old-project: automat
ms.assetid: af9f85fa-b123-49da-99c7-552cd03197c0
ms.author: windowsdriverdev
ms.date: 5/4/2018
ms.keywords: VARIANT_UserMarshal64, VARIANT_UserMarshal64 function [Automation], automat.variant_usermarshal64, oaidl/VARIANT_UserMarshal64
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps | UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps | UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: VARKIND
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	OleAut32.dll
api_name:
-	VARIANT_UserMarshal64
product: Windows
targetos: Windows
req.lib: OleAut32.lib
req.dll: OleAut32.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# VARIANT_UserMarshal64 function


## -description


Marshals a <a href="https://msdn.microsoft.com/library/windows/hardware/mt138335">VARIANT</a> object into the RPC buffer.


## -parameters




### -param

TBD




#### - pBuffer [in, out]

The current buffer. This pointer may or may not be aligned on entry.


#### - pFlags [in]

The data used by RPC.


#### - pVariant [in]

The object.


## -returns



The value obtained from the returned <b>HRESULT</b> value is one of the following.



<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG
</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVariant</i> parameter is not valid.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_X_NULL_REF_POINTER
</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVariant</i> parameter is null.


</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DISP_E_BADVARTYPE
</b></dt>
</dl>
</td>
<td width="60%">
The input parameter is not a valid type of variant.

</td>
</tr>
</table>
 


