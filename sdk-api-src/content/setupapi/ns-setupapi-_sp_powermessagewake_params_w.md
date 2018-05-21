---
UID: NS:setupapi._SP_POWERMESSAGEWAKE_PARAMS_W
title: "_SP_POWERMESSAGEWAKE_PARAMS_W"
author: windows-driver-content
description: An SP_POWERMESSAGEWAKE_PARAMS structure corresponds to a DIF_POWERMESSAGEWAKE installation request.
old-location: devinst\sp_powermessagewake_params.htm
old-project: devinst
ms.assetid: 464919bb-c146-4d29-890f-c680a1aa06b2
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PSP_POWERMESSAGEWAKE_PARAMS_W, PSP_POWERMESSAGEWAKE_PARAMS, PSP_POWERMESSAGEWAKE_PARAMS structure pointer [Device and Driver Installation], SP_POWERMESSAGEWAKE_PARAMS, SP_POWERMESSAGEWAKE_PARAMS structure [Device and Driver Installation], SP_POWERMESSAGEWAKE_PARAMS_W, _SP_POWERMESSAGEWAKE_PARAMS_W, devinst.sp_powermessagewake_params, di-struct_ac0928d6-b3df-4bf2-8304-a6b03eaa63a8.xml, setupapi/PSP_POWERMESSAGEWAKE_PARAMS, setupapi/SP_POWERMESSAGEWAKE_PARAMS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: setupapi.h
req.include-header: Setupapi.h
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
req.typenames: SP_POWERMESSAGEWAKE_PARAMS_W, *PSP_POWERMESSAGEWAKE_PARAMS_W
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	setupapi.h
api_name:
-	SP_POWERMESSAGEWAKE_PARAMS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# _SP_POWERMESSAGEWAKE_PARAMS_W structure


## -description


An SP_POWERMESSAGEWAKE_PARAMS structure corresponds to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff543709">DIF_POWERMESSAGEWAKE</a> installation request.


## -struct-fields




### -field ClassInstallHeader

An install request header that contains the header size and the DIF code for the request. See <a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>.


### -field PowerMessageWake

Buffer that contains a string of custom text. Windows displays this text on the power management page of the device properties display in Device Manager.


## -remarks



Windows only sends the DIF_POWERMESSAGEWAKE request if the drivers for the device support power management.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff543709">DIF_POWERMESSAGEWAKE</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>
 

 
