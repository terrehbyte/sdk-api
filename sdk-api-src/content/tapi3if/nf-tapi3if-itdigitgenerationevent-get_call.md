---
UID: NF:tapi3if.ITDigitGenerationEvent.get_Call
title: ITDigitGenerationEvent::get_Call
author: windows-driver-content
description: The get_Call method returns an ITCallInfo interface pointer for the call on which the event is required.
old-location: tapi3\itdigitgenerationevent_get_call.htm
old-project: Tapi
ms.assetid: b0f4281f-e1df-4be9-acfc-5482044eb44b
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITDigitGenerationEvent interface [TAPI 2.2],get_Call method, ITDigitGenerationEvent.get_Call, ITDigitGenerationEvent::get_Call, _tapi3_itdigitgenerationevent_get_call, get_Call, get_Call method [TAPI 2.2], get_Call method [TAPI 2.2],ITDigitGenerationEvent interface, tapi3.itdigitgenerationevent_get_call, tapi3if/ITDigitGenerationEvent::get_Call
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
-	Tapi3.dll
api_name:
-	ITDigitGenerationEvent.get_Call
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITDigitGenerationEvent::get_Call


## -description


The 
<b>get_Call</b> method returns an 
<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a> interface pointer for the call on which the event is required.


## -parameters




### -param ppCallInfo [out]

Pointer to 
<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a> interface.


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
The <i>ppCallInfo</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/5209d4a1-e05b-453e-8896-2dc71f0b9af0">ITCallInfo</a>



<a href="https://msdn.microsoft.com/788eee9c-b885-4b94-b259-694353c0f63a">ITDigitGenerationEvent</a>
 

 
