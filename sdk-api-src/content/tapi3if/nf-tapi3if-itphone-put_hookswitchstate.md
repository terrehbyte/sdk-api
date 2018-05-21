---
UID: NF:tapi3if.ITPhone.put_HookSwitchState
title: ITPhone::put_HookSwitchState
author: windows-driver-content
description: The put_HookSwitchState method sets the current hookswitch state for a particular hookswitch device on the phone.
old-location: tapi3\itphone_put_hookswitchstate.htm
old-project: Tapi
ms.assetid: ab0bcd30-6985-4f53-a39d-90230421b6f4
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITPhone interface [TAPI 2.2],put_HookSwitchState method, ITPhone.put_HookSwitchState, ITPhone::put_HookSwitchState, _tapi3_itphone_put_hookswitchstate, put_HookSwitchState, put_HookSwitchState method [TAPI 2.2], put_HookSwitchState method [TAPI 2.2],ITPhone interface, tapi3.itphone_put_hookswitchstate, tapi3if/ITPhone::put_HookSwitchState
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
-	ITPhone.put_HookSwitchState
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITPhone::put_HookSwitchState


## -description


The 
<b>put_HookSwitchState</b> method sets the current hookswitch state for a particular hookswitch device on the phone.

The application must call 
<a href="https://msdn.microsoft.com/d9efe2f7-3628-4e1f-b554-a6889d82a973">ITPhone::Open</a> before invoking this method; otherwise, the invocation fails.


## -parameters




### -param HookSwitchDevice [in]

The 
<a href="https://msdn.microsoft.com/20b17e2f-f745-41ef-91ac-d2ab21d43695">PHONE_HOOK_SWITCH_DEVICE</a> descriptor for the hookswitch type.


### -param HookSwitchState [in]

The 
<a href="https://msdn.microsoft.com/c9501a3f-1aaa-4d58-aca1-5ef00c31d195">PHONE_HOOK_SWITCH_STATE</a> descriptor for the hookswitch status.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Typically, speakerphones and headsets have application-settable hookswitch states, and handsets do not, but this feature is TSP-dependent.




## -see-also




<a href="https://msdn.microsoft.com/94dff33c-67a1-4df8-9ef5-2b6524438f6f">ITPhone</a>



<a href="https://msdn.microsoft.com/4560b447-45af-482a-b97b-dd0cbdb52466">get_HookSwitchState</a>
 

 
