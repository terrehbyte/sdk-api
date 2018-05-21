---
UID: NF:cfgmgr32.CM_Get_Device_Interface_PropertyW
title: CM_Get_Device_Interface_PropertyW function
author: windows-driver-content
description: The CM_Get_Device_Interface_Property function retrieves a device property that is set for a device interface.
old-location: devinst\cm_get_device_interface_property.htm
old-project: devinst
ms.assetid: 581286BF-F20E-4766-BF0C-5D6B34032358
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Get_Device_Interface_Property, CM_Get_Device_Interface_Property function [Device and Driver Installation], CM_Get_Device_Interface_PropertyA, CM_Get_Device_Interface_PropertyW, cfgmgr32/CM_Get_Device_Interface_Property, cfgmgr32/CM_Get_Device_Interface_PropertyA, cfgmgr32/CM_Get_Device_Interface_PropertyW, devinst.cm_get_device_interface_property
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Universal
req.target-min-winverclnt: Available in Microsoft Windows Vista and later versions of Windows.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: CM_Get_Device_Interface_PropertyW (Unicode) and CM_Get_Device_Interface_PropertyA (ANSI)
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
-	Cfgmgr32.lib
-	Cfgmgr32.dll
-	API-MS-Win-Devices-Config-L1-1-0.dll
-	API-MS-Win-Devices-Config-L1-1-1.dll
-	CfgMgr32.dll
api_name:
-	CM_Get_Device_Interface_Property
-	CM_Get_Device_Interface_PropertyA
-	CM_Get_Device_Interface_PropertyW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Get_Device_Interface_PropertyW function


## -description


The <b>CM_Get_Device_Interface_Property</b> function retrieves a device property that is set for a device interface.


## -parameters




### -param pszDeviceInterface [in]

Pointer to a string that identifies the device interface instance to retrieve the property from.


### -param PropertyKey [in]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a> structure that represents the device interface property key of the device interface property to retrieve.


### -param PropertyType [out]

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff543546">DEVPROPTYPE</a>-typed variable that receives the property-data-type identifier of the requested device interface property. The property-data-type identifier is a bitwise OR between a base-data-type identifier and, if the base-data type is modified, a property-data-type modifier.


### -param PropertyBuffer [out]

A pointer to a buffer that receives the requested device interface property. <b>CM_Get_Device_Interface_Property</b> retrieves the requested property only if the buffer is large enough to hold all the property value data. The pointer can be NULL.


### -param PropertyBufferSize [in, out]

The size, in bytes, of the <i>PropertyBuffer</i> buffer. If <i>PropertyBuffer</i> is set to NULL, <i>*PropertyBufferSize</i> must be set to zero. As output, if the buffer is not large enough to hold all the property value data, <b>CM_Get_Device_Interface_Property</b> returns the size of the data, in bytes, in <i>*PropertyBufferSize</i>.


### -param ulFlags [in]

Reserved. Must be set to zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



<b>CM_Get_Device_Interface_Property</b> is part of the <a href="devinst.unified_device_property_model__windows_vista_and_later_">Unified Device Property Model</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff551122">SetupDiGetDeviceInterfaceProperty</a>
 

 
