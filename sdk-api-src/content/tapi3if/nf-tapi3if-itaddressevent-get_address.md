---
UID: NF:tapi3if.ITAddressEvent.get_Address
title: ITAddressEvent::get_Address
author: windows-driver-content
description: The get_Address method gets a pointer to the ITAddress object involved in an event.
old-location: tapi3\itaddressevent_get_address.htm
old-project: Tapi
ms.assetid: 5616205a-922d-4d86-8a8d-89672288563a
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITAddressEvent interface [TAPI 2.2],get_Address method, ITAddressEvent.get_Address, ITAddressEvent::get_Address, _tapi3_itaddressevent_get_address, get_Address, get_Address method [TAPI 2.2], get_Address method [TAPI 2.2],ITAddressEvent interface, tapi3.itaddressevent_get_address, tapi3if/ITAddressEvent::get_Address
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
-	ITAddressEvent.get_Address
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITAddressEvent::get_Address


## -description


The 
<b>get_Address</b> method gets a pointer to the 
<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a> object involved in an event.


## -parameters




### -param ppAddress [out]

Pointer to an 
<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a> interface.


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
The <i>ppAddress</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -remarks



TAPI calls the <b>AddRef</b> method on the 
<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a> interface returned by <b>ITAddressEvent::get_Address</b>. The application must call <b>Release</b> on the 
<b>ITAddress</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/ab6db262-f99e-4027-9525-7597fcf02e72">Address Object</a>



<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a>



<a href="https://msdn.microsoft.com/340d938a-a107-4317-af65-3dca98102767">ITAddressEvent</a>
 

 
