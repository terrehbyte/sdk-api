---
UID: NF:tapi3if.ITCallMediaEvent.get_Event
title: ITCallMediaEvent::get_Event
author: windows-driver-content
description: The get_Event method gets the call media event indicator.
old-location: tapi3\itcallmediaevent_get_event.htm
old-project: Tapi
ms.assetid: 3dd6210f-e904-46c5-8fc3-50a62b8754ed
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITCallMediaEvent interface [TAPI 2.2],get_Event method, ITCallMediaEvent.get_Event, ITCallMediaEvent::get_Event, _tapi3_itcallmediaevent_get_event, get_Event, get_Event method [TAPI 2.2], get_Event method [TAPI 2.2],ITCallMediaEvent interface, tapi3.itcallmediaevent_get_event, tapi3if/ITCallMediaEvent::get_Event
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
-	ITCallMediaEvent.get_Event
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITCallMediaEvent::get_Event


## -description


The 
<b>get_Event</b> method gets the call media event indicator.


## -parameters




### -param pCallMediaEvent [out]

Pointer to 
<a href="https://msdn.microsoft.com/835759f4-652b-4d01-911a-e580bb29d292">CALL_MEDIA_EVENT</a> indicator.


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
The <i>pCallMediaEvent</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -remarks



Call media events are a crucial indicator of whether certain operations can be performed. For example, when 
<b>IVideoWindow</b> is exposed on the 
<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal object</a>, until the CME_STREAM_ACTIVE is received only the 
<b>put_Visible</b> method will succeed. For more information about <b>IVideoWindow</b> and <b>put_Visible</b>, see the DirectX documentation. 




## -see-also




<a href="https://msdn.microsoft.com/835759f4-652b-4d01-911a-e580bb29d292">CALL_MEDIA_EVENT</a>



<a href="https://msdn.microsoft.com/67c063ba-8b12-40d6-9011-923bdee8b214">Call Object</a>



<a href="https://msdn.microsoft.com/db55ff03-9271-4a94-9cba-a3ef0282b7b6">ITCallMediaEvent</a>
 

 
