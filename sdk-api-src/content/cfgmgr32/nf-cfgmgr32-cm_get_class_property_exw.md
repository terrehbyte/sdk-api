---
UID: NF:cfgmgr32.CM_Get_Class_Property_ExW
title: CM_Get_Class_Property_ExW function
author: windows-driver-content
description: The CM_Get_Class_Property_ExW function retrieves a device property that is set for a device interface class or device setup class.
old-location: devinst\cm_get_class_property_exw.htm
old-project: devinst
ms.assetid: 580E055C-B731-4168-8051-81BD5ACB4EFC
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Get_Class_Property_ExW, CM_Get_Class_Property_ExW function [Device and Driver Installation], cfgmgr32/CM_Get_Class_Property_ExW, devinst.cm_get_class_property_exw
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 10 and later versions of Windows.
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
req.typenames: CM_NOTIFY_ACTION, *PCM_NOTIFY_ACTION
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	LibDef
api_location:
-	Cfgmgr32.lib
-	Cfgmgr32.dll
api_name:
-	CM_Get_Class_Property_ExW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Get_Class_Property_ExW function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/hh780216">CM_Get_Class_Property</a> instead.]

The <b>CM_Get_Class_Property_ExW</b> function retrieves a device property that is set for a <a href="https://msdn.microsoft.com/C989D2D3-E8DE-4D64-86EE-3D3B3906390D">device interface class</a> or <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a>.


## -parameters




### -param ClassGUID [in]

Pointer to the GUID that identifies the <a href="https://msdn.microsoft.com/C989D2D3-E8DE-4D64-86EE-3D3B3906390D">device interface class</a> or <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a> for which to retrieve a device property that is set for the device class. For information about specifying the class type, see the <i>ulFlags</i> parameter.


### -param PropertyKey [in]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a> structure that represents the device property key of the requested device class property.


### -param PropertyType [out]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff543546">DEVPROPTYPE</a>-typed variable that receives the property-data-type identifier of the requested device class property, where the property-data-type identifier is the bitwise OR between a base-data-type identifier and, if the base data type is modified, a property-data-type modifier.


### -param PropertyBuffer [out]

Pointer to a buffer that receives the requested device class property. <b>CM_Get_Class_Property_ExW</b> retrieves the requested property value only if the buffer is large enough to hold all the property value data. The pointer can be NULL.


### -param PropertyBufferSize [in, out]

The size, in bytes, of the <i>PropertyBuffer</i> buffer. If the <i>PropertyBuffer</i> parameter is set to NULL, <i>*PropertyBufferSize</i> must be set to zero. As output, if the buffer is not large enough to hold all the property value data, <b>CM_Get_Class_Property_ExW</b> returns the size of the data, in bytes, in <i>*PropertyBufferSize</i>.


### -param ulFlags [in]

Class property flags:





#### CM_CLASS_PROPERTY_INSTALLER

<i>ClassGUID</i> specifies a device setup class. Do not combine with CM_CLASS_PROPERTY_INTERFACE.



#### CM_CLASS_PROPERTY_INTERFACE

<i>ClassGUID</i> specifies a device interface class. Do not combine with CM_CLASS_PROPERTY_INSTALLER.


### -param hMachine [in]

Caller-supplied machine handle, obtained from a previous call to <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



<b>CM_Get_Class_Property_ExW</b> is part of the <a href="devinst.unified_device_property_model__windows_vista_and_later_">Unified Device Property Model</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551086">SetupDiGetClassProperty</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551090">SetupDiGetClassPropertyEx</a>
 

 
