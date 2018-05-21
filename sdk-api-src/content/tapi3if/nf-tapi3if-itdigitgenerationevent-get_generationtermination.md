---
UID: NF:tapi3if.ITDigitGenerationEvent.get_GenerationTermination
title: ITDigitGenerationEvent::get_GenerationTermination
author: windows-driver-content
description: The get_GenerationTermination method gets the digit or digits that indicate the end of the generated digit series.
old-location: tapi3\itdigitgenerationevent_get_generationtermination.htm
old-project: Tapi
ms.assetid: 70e8c932-a157-455e-b340-d7e4eb19823c
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITDigitGenerationEvent interface [TAPI 2.2],get_GenerationTermination method, ITDigitGenerationEvent.get_GenerationTermination, ITDigitGenerationEvent::get_GenerationTermination, _tapi3_itdigitgenerationevent_get_generationtermination, get_GenerationTermination, get_GenerationTermination method [TAPI 2.2], get_GenerationTermination method [TAPI 2.2],ITDigitGenerationEvent interface, tapi3.itdigitgenerationevent_get_generationtermination, tapi3if/ITDigitGenerationEvent::get_GenerationTermination
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
-	ITDigitGenerationEvent.get_GenerationTermination
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITDigitGenerationEvent::get_GenerationTermination


## -description


The 
<b>get_GenerationTermination</b> method gets the digit or digits that indicate the end of the generated digit series.


## -parameters




### -param plGenerationTermination [out]

Pointer to digit or digits that indicate the end of the generated digit series.


## -returns



This method can return one of these values.

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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>plGenerationTermination</i> parameter is not a valid pointer.

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
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/788eee9c-b885-4b94-b259-694353c0f63a">ITDigitGenerationEvent</a>
 

 
