---
UID: NC:tapi.PHONECALLBACK
title: PHONECALLBACK
author: windows-driver-content
description: The phoneCallback function is a placeholder for the application-supplied function name.
old-location: tapi2\phonecallbackfunc.htm
old-project: Tapi
ms.assetid: 169ac08a-7584-4d43-abb3-eb83eeb48406
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: PHONECALLBACK, PHONECALLBACK callback function [TAPI 2.2], _tapi2_phonecallbackfunc, phoneCallback, phoneCallback callback, tapi/PHONECALLBACK, tapi2.phonecallbackfunc
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: tapi.h
req.include-header: 
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
req.typenames: FLICK_POINT
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	Tapi.h
api_name:
-	PHONECALLBACK
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows XP with SP1 and later
---

# PHONECALLBACK callback function


## -description


The 
<b>phoneCallback</b> function is a placeholder for the application-supplied function name.


## -parameters




### -param hDevice

Handle to a phone device associated with the callback.


### -param dwMessage


### -param dwInstance


### -param dwParam1

Parameter for the message.


### -param dwParam2

Parameter for the message.


### -param dwParam3

Parameter for the message.


#### - dwCallbackInstance

Callback instance data passed back to the application in the callback. This <b>DWORD</b> is not interpreted by TAPI.


#### - dwMsg

Line or call device message.


## -returns



This callback function does not return a value.




## -remarks



For more information about the parameters passed to this callback function, see 
<a href="https://msdn.microsoft.com/d302819e-c522-470a-be5e-52625c9223a4">TAPI Messages</a>.

All callbacks occur in the application's context. The callback function must reside in a dynamic-link library (DLL) or application module and be exported in the module-definition file.


