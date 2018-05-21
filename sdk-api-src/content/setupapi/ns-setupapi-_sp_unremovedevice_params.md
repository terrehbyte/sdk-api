---
UID: NS:setupapi._SP_UNREMOVEDEVICE_PARAMS
title: "_SP_UNREMOVEDEVICE_PARAMS"
author: windows-driver-content
description: An SP_UNREMOVEDEVICE_PARAMS structure corresponds to a DIF_UNREMOVE installation request.
old-location: devinst\sp_unremovedevice_params.htm
old-project: devinst
ms.assetid: 89f5e2a9-5336-421f-b781-688588695027
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PSP_UNREMOVEDEVICE_PARAMS, PSP_UNREMOVEDEVICE_PARAMS, PSP_UNREMOVEDEVICE_PARAMS structure pointer [Device and Driver Installation], SP_UNREMOVEDEVICE_PARAMS, SP_UNREMOVEDEVICE_PARAMS structure [Device and Driver Installation], _SP_UNREMOVEDEVICE_PARAMS, devinst.sp_unremovedevice_params, di-struct_bcd98087-c502-40d6-81a7-5154340ce406.xml, setupapi/PSP_UNREMOVEDEVICE_PARAMS, setupapi/SP_UNREMOVEDEVICE_PARAMS"
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
req.typenames: SP_UNREMOVEDEVICE_PARAMS, *PSP_UNREMOVEDEVICE_PARAMS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	setupapi.h
api_name:
-	SP_UNREMOVEDEVICE_PARAMS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# _SP_UNREMOVEDEVICE_PARAMS structure


## -description


An SP_UNREMOVEDEVICE_PARAMS structure corresponds to a DIF_UNREMOVE installation request.


## -struct-fields




### -field ClassInstallHeader

An install request header that contains the header size and the DIF code for the request. See <a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>. 


### -field Scope

A flag that indicates the scope of the unremove operation. This flag must always be set to DI_UNREMOVEDEVICE_CONFIGSPECIFIC. 


### -field HwProfile

The hardware profile ID for profile-specific changes. Zero specifies the current hardware profile. 


## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff543728">DIF_UNREMOVE</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552193">SetupDiUnremoveDevice</a>
 

 
