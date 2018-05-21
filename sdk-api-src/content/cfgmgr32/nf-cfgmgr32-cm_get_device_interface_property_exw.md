---
UID: NF:cfgmgr32.CM_Get_Device_Interface_Property_ExW
title: CM_Get_Device_Interface_Property_ExW function
author: windows-driver-content
description: The CM_Get_Device_Interface_Property_ExW function retrieves a device property that is set for a device interface.
old-location: devinst\cm_get_device_interface_property_exw.htm
old-project: devinst
ms.assetid: A367AF27-BF99-4322-9D11-8792AA2863B9
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Get_Device_Interface_Property_ExW, CM_Get_Device_Interface_Property_ExW function [Device and Driver Installation], cfgmgr32/CM_Get_Device_Interface_Property_ExW, devinst.cm_get_device_interface_property_exw
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
-	DllExport
api_location:
-	CfgMgr32.dll
-	API-MS-Win-Devices-Config-L1-1-0.dll
-	API-MS-Win-Devices-Config-L1-1-1.dll
api_name:
-	CM_Get_Device_Interface_Property_ExW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: CfgMgr32.dll
req.irql: 
---

# CM_Get_Device_Interface_Property_ExW function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/hh780218">CM_Get_Device_Interface_Property</a> instead.]

The <b>CM_Get_Device_Interface_Property_ExW</b> function retrieves a device property that is set for a device interface.


## -parameters




### -param pszDeviceInterface [in]

Pointer to a string that identifies the device interface instance to retrieve the property from.


### -param PropertyKey [in]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a> structure that represents the device interface property key of the device interface property to retrieve.


### -param PropertyType [out]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff543546">DEVPROPTYPE</a>-typed variable that receives the property-data-type identifier of the requested device interface property. The property-data-type identifier is a bitwise OR between a base-data-type identifier and, if the base-data type is modified, a property-data-type modifier.


### -param PropertyBuffer [out]

A pointer to a buffer that receives the requested device interface property. <b>CM_Get_Device_Interface_Property_ExW</b> retrieves the requested property only if the buffer is large enough to hold all the property value data. The pointer can be NULL.


### -param PropertyBufferSize [in, out]

The size, in bytes, of the <i>PropertyBuffer</i> buffer. If <i>PropertyBuffer</i> is set to NULL, <i>*PropertyBufferSize</i> must be set to zero. As output, if the buffer is not large enough to hold all the property value data, <b>CM_Get_Device_Interface_Property_ExW</b> returns the size of the data, in bytes, in <i>*PropertyBufferSize</i>.


### -param ulFlags [in]

Reserved. Must be set to zero.


### -param hMachine [in, optional]

Caller-supplied machine handle, obtained from a previous call to <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



<b>CM_Get_Device_Interface_Property_ExW</b> is part of the <a href="devinst.unified_device_property_model__windows_vista_and_later_">Unified Device Property Model</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551122">SetupDiGetDeviceInterfaceProperty</a>
 

 
