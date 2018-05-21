---
UID: NF:tapi3if.ITStreamControl.EnumerateStreams
title: ITStreamControl::EnumerateStreams
author: windows-driver-content
description: The EnumerateStreams method enumerates currently available media streams. Provided for C and C++ applications. Automation client applications such as Visual Basic must use the get_Streams method.
old-location: tapi3\itstreamcontrol_enumeratestreams.htm
old-project: Tapi
ms.assetid: de018f3e-d3b9-4093-a2b5-4929ac4d1d2a
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: EnumerateStreams, EnumerateStreams method [TAPI 2.2], EnumerateStreams method [TAPI 2.2],ITStreamControl interface, ITStreamControl interface [TAPI 2.2],EnumerateStreams method, ITStreamControl.EnumerateStreams, ITStreamControl::EnumerateStreams, _tapi3_itstreamcontrol_enumeratestreams, tapi3.itstreamcontrol_enumeratestreams, tapi3if/ITStreamControl::EnumerateStreams
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: TERMINAL_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	tapi3if.h
api_name:
-	ITStreamControl.EnumerateStreams
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITStreamControl::EnumerateStreams


## -description


The <b>EnumerateStreams</b> method enumerates currently available media streams. Provided for C and C++ applications. Automation client applications such as Visual Basic must use the 
<a href="https://msdn.microsoft.com/4d001f5a-7731-47b9-8c68-e4dd2d0bf02f">get_Streams</a> method.


## -parameters




### -param ppEnumStream [out]

Pointer to pointer for 
<a href="https://msdn.microsoft.com/52e8c040-8bc5-4c9c-a697-ec05164adea2">IEnumStream</a> enumerator.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppEnumStream</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -remarks



TAPI calls the <a href="_com_iunknown_addref">AddRef</a> method on the 
<a href="https://msdn.microsoft.com/52e8c040-8bc5-4c9c-a697-ec05164adea2">IEnumStream</a> interface returned by <b>ITStreamControl::EnumerateStreams</b>. The application must call <a href="_com_iunknown_release">Release</a> on the 
<b>IEnumStream</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/12b9457a-7afb-4348-93a2-28728c673929">ITStreamControl</a>



<a href="https://msdn.microsoft.com/53b7bcbd-571a-44da-a6db-10d4c3e5d30a">Media Service Provider Interface (MSPI)</a>
 

 
