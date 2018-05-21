---
UID: NF:tapi3if.ITCallStateEvent.get_CallbackInstance
title: ITCallStateEvent::get_CallbackInstance
author: windows-driver-content
description: The get_CallbackInstance method gets a pointer to the callback instance associated with this event.
old-location: tapi3\itcallstateevent_get_callbackinstance.htm
old-project: Tapi
ms.assetid: e4add561-94be-44e2-84bb-89d1e5e98969
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITCallStateEvent interface [TAPI 2.2],get_CallbackInstance method, ITCallStateEvent.get_CallbackInstance, ITCallStateEvent::get_CallbackInstance, _tapi3_itcallstateevent_get_callbackinstance, get_CallbackInstance, get_CallbackInstance method [TAPI 2.2], get_CallbackInstance method [TAPI 2.2],ITCallStateEvent interface, tapi3.itcallstateevent_get_callbackinstance, tapi3if/ITCallStateEvent::get_CallbackInstance
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
-	ITCallStateEvent.get_CallbackInstance
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITCallStateEvent::get_CallbackInstance


## -description


The 
<b>get_CallbackInstance</b> method gets a pointer to the callback instance associated with this event.


## -parameters




### -param plCallbackInstance [out]

Pointer to callback instance returned by 
<a href="https://msdn.microsoft.com/335deb2c-7700-4101-b6fa-f7fe0f248307">ITTAPI::RegisterCallNotifications</a>.


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
The <i>plCallbackInstance</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/67c063ba-8b12-40d6-9011-923bdee8b214">Call Object</a>



<a href="https://msdn.microsoft.com/0885ef81-726d-41ca-be8c-b3ff2e02fc3c">ITCallStateEvent</a>



<a href="https://msdn.microsoft.com/335deb2c-7700-4101-b6fa-f7fe0f248307">ITTAPI::RegisterCallNotifications</a>
 

 
