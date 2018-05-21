---
UID: NF:cfgmgr32.CM_Get_Device_Interface_Property_Keys_ExW
title: CM_Get_Device_Interface_Property_Keys_ExW function
author: windows-driver-content
description: The CM_Get_Device_Interface_Property_Keys_ExW function retrieves an array of device property keys that represent the device properties that are set for a device interface.
old-location: devinst\cm_get_device_interface_property_keys_exw.htm
old-project: devinst
ms.assetid: 52EEF50F-4559-4C22-BE33-1F87E469BB47
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Get_Device_Interface_Property_Keys_ExW, CM_Get_Device_Interface_Property_Keys_ExW function [Device and Driver Installation], cfgmgr32/CM_Get_Device_Interface_Property_Keys_ExW, devinst.cm_get_device_interface_property_keys_exw
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
-	CM_Get_Device_Interface_Property_Keys_ExW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Get_Device_Interface_Property_Keys_ExW function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/hh780219">CM_Get_Device_Interface_Property_Keys</a> instead.]

The <b>CM_Get_Device_Interface_Property_Keys_ExW</b> function retrieves an array of device property keys that represent the device properties that are set for a device interface.


## -parameters




### -param pszDeviceInterface [in]

Pointer to a string that identifies the device interface instance to retrieve the property keys from.


### -param PropertyKeyArray [out, optional]

Pointer to a buffer that receives an array of <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a>-typed values, where each value is a device property key that represents a device property that is set for the device interface. The pointer is optional and can be NULL


### -param PropertyKeyCount [in, out]

The size, in <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a>-typed units, of the <i>PropertyKeyArray</i> buffer. If <i>PropertyKeyArray</i> is set to NULL, <i>*PropertyKeyCount</i> must be set to zero.  As output, if <i>PropertyKeyArray</i> is not large enough to hold all the property key data, <b>CM_Get_Device_Interface_Property_Keys_ExW</b> returns the count of the keys, in <i>*PropertyKeyCount</i>.


### -param ulFlags [in]

Reserved. Must be set to zero.


### -param hMachine [in, optional]

Caller-supplied machine handle, obtained from a previous call to <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



<b>CM_Get_Device_Interface_Property_Keys_ExW</b> is part of the <a href="devinst.unified_device_property_model__windows_vista_and_later_">Unified Device Property Model</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551959">SetupDiGetDeviceInterfacePropertyKeys</a>
 

 
