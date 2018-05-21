---
UID: NF:tapi3if.ITAutomatedPhoneControl.StartRinger
title: ITAutomatedPhoneControl::StartRinger
author: windows-driver-content
description: The StartRinger method starts the phone's ringer, specifying the ring mode and the duration of the ring.
old-location: tapi3\itautomatedphonecontrol_startringer.htm
old-project: Tapi
ms.assetid: bf94aab7-6b12-43f8-b49f-a7cf6617dd57
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITAutomatedPhoneControl interface [TAPI 2.2],StartRinger method, ITAutomatedPhoneControl.StartRinger, ITAutomatedPhoneControl::StartRinger, StartRinger, StartRinger method [TAPI 2.2], StartRinger method [TAPI 2.2],ITAutomatedPhoneControl interface, _tapi3_itautomatedphonecontrol_startringer, tapi3.itautomatedphonecontrol_startringer, tapi3if/ITAutomatedPhoneControl::StartRinger
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
-	ITAutomatedPhoneControl.StartRinger
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITAutomatedPhoneControl::StartRinger


## -description


The 
<b>StartRinger</b> method starts the phone's ringer, specifying the ring mode and the duration of the ring.


## -parameters




### -param lRingMode [in]

Ring mode. The exact meaning of this value is device-dependent. For more information, see the following Remarks section.


### -param lDuration [in]

Length of ring.


## -returns



If the method succeeds, it returns S_OK. Otherwise, it returns an error value.




## -remarks



If you specify the value zero in the <i>lRingMode</i> parameter, and the phone doesn't have a ringer device, the 
<b>StartRinger</b> method attempts to play the ringing sound on the system's default audio render device. Examples of default devices include sound card speakers and a USB phone's audio render device. For more information, see 
<a href="https://msdn.microsoft.com/7a73d5ff-d08a-46e6-b4ad-4f3b973967a7">PHONECAPS_LONG</a>.




## -see-also




<a href="https://msdn.microsoft.com/60d4f079-75ee-4aeb-9e7c-0b16d90da754">ITAutomatedPhoneControl</a>
 

 
