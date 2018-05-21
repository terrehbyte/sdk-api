---
UID: NF:tapi3if.ITRequestEvent.get_CalledParty
title: ITRequestEvent::get_CalledParty
author: windows-driver-content
description: The get_CalledParty method gets the called party.
old-location: tapi3\itrequestevent_get_calledparty.htm
old-project: Tapi
ms.assetid: 0dfbf033-83cf-4e2c-b107-963c10595ee5
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITRequestEvent interface [TAPI 2.2],get_CalledParty method, ITRequestEvent.get_CalledParty, ITRequestEvent::get_CalledParty, _tapi3_itrequestevent_get_calledparty, get_CalledParty, get_CalledParty method [TAPI 2.2], get_CalledParty method [TAPI 2.2],ITRequestEvent interface, tapi3.itrequestevent_get_calledparty, tapi3if/ITRequestEvent::get_CalledParty
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
-	ITRequestEvent.get_CalledParty
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITRequestEvent::get_CalledParty


## -description


The 
<b>get_CalledParty</b> method gets the called party.


## -parameters




### -param ppCalledParty [out]

Pointer to a <b>BSTR</b> containing the called party identifier.


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
The <i>ppCalledParty</i> is not a valid pointer.

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
 




## -remarks



The application must use 
<a href="8f230ee3-5f6e-4cb9-a910-9c90b754dcd3">SysFreeString</a> to free the memory allocated for the <i>ppCalledParty</i> parameter.
			




## -see-also




<a href="https://msdn.microsoft.com/69f9b504-be01-4167-8002-32a8e86bab0f">ITRequestEvent</a>
 

 
