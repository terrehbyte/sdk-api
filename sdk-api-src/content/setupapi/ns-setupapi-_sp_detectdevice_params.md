---
UID: NS:setupapi._SP_DETECTDEVICE_PARAMS
title: "_SP_DETECTDEVICE_PARAMS"
author: windows-driver-content
description: An SP_DETECTDEVICE_PARAMS structure corresponds to a DIF_DETECT installation request.
old-location: devinst\sp_detectdevice_params.htm
old-project: devinst
ms.assetid: 77682651-217f-4e3a-9d0e-0a93d315de53
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PSP_DETECTDEVICE_PARAMS, PSP_DETECTDEVICE_PARAMS, PSP_DETECTDEVICE_PARAMS structure pointer [Device and Driver Installation], SP_DETECTDEVICE_PARAMS, SP_DETECTDEVICE_PARAMS structure [Device and Driver Installation], _SP_DETECTDEVICE_PARAMS, devinst.sp_detectdevice_params, di-struct_6de1fd38-be9a-42e6-ae10-5825aef12880.xml, setupapi/PSP_DETECTDEVICE_PARAMS, setupapi/SP_DETECTDEVICE_PARAMS"
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
req.typenames: SP_DETECTDEVICE_PARAMS, *PSP_DETECTDEVICE_PARAMS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	setupapi.h
api_name:
-	SP_DETECTDEVICE_PARAMS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# _SP_DETECTDEVICE_PARAMS structure


## -description


An SP_DETECTDEVICE_PARAMS structure corresponds to a DIF_DETECT installation request.


## -struct-fields




### -field ClassInstallHeader

An install request header that contains the size of the header and the DIF code for the request. See <a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>. 


### -field DetectProgressNotify

A callback routine that displays a progress bar for the device detection operation. The callback routine is supplied by the <a href="devinst.device_installation_components">device installation component</a> that sends the <a href="https://msdn.microsoft.com/library/windows/hardware/ff543674">DIF_DETECT</a> request. The callback has the following prototype:

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>typedef BOOL (CALLBACK* PDETECT_PROGRESS_NOTIFY)(
    IN PVOID ProgressNotifyParam,
    IN DWORD DetectComplete
    );</pre>
</td>
</tr>
</table></span></div>
<i>ProgressNotifyParam</i> is an opaque "handle" that identifies the detection operation. This value is supplied by the <a href="devinst.device_installation_components">device installation component</a> that sent the DIF_DETECT request. 

<i>DetectComplete</i> is a value between 0 and 100 that indicates the percent completion. The class installer increments this value at various stages of its detection activities, to notify the user of its progress.


### -field ProgressNotifyParam

The opaque <b>ProgressNotifyParam</b> "handle" that the class installer passes to the progress callback routine.


## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff543674">DIF_DETECT</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552340">SP_CLASSINSTALL_HEADER</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a>
 

 
