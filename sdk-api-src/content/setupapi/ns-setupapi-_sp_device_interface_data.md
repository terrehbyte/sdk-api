---
UID: NS:setupapi._SP_DEVICE_INTERFACE_DATA
title: "_SP_DEVICE_INTERFACE_DATA"
author: windows-driver-content
description: An SP_DEVICE_INTERFACE_DATA structure defines a device interface in a device information set.
old-location: devinst\sp_device_interface_data.htm
old-project: devinst
ms.assetid: df142e95-aa1c-4d3e-90c6-bac86effbd5d
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PSP_DEVICE_INTERFACE_DATA, PSP_DEVICE_INTERFACE_DATA, PSP_DEVICE_INTERFACE_DATA structure pointer [Device and Driver Installation], SP_DEVICE_INTERFACE_DATA, SP_DEVICE_INTERFACE_DATA structure [Device and Driver Installation], SP_INTERFACE_DEVICE_DATA, _SP_DEVICE_INTERFACE_DATA, devinst.sp_device_interface_data, di-struct_6ad1a986-b29c-4adc-af28-e8895eee5ac4.xml, setupapi/PSP_DEVICE_INTERFACE_DATA, setupapi/SP_DEVICE_INTERFACE_DATA"
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
req.typenames: SP_DEVICE_INTERFACE_DATA, *PSP_DEVICE_INTERFACE_DATA
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	setupapi.h
api_name:
-	SP_DEVICE_INTERFACE_DATA
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# _SP_DEVICE_INTERFACE_DATA structure


## -description


An SP_DEVICE_INTERFACE_DATA structure defines a device interface in a device information set.


## -struct-fields




### -field cbSize

The size, in bytes, of the SP_DEVICE_INTERFACE_DATA structure. For more information, see the Remarks section. 


### -field InterfaceClassGuid

The GUID for the class to which the device interface belongs.


### -field Flags

Can be one or more of the following:





#### SPINT_ACTIVE

The interface is active (enabled).



#### SPINT_DEFAULT

The interface is the default interface for the device class.



#### SPINT_REMOVED

The interface is removed.


### -field Reserved

Reserved. Do not use.


## -remarks



A SetupAPI function that takes an instance of the SP_DEVICE_INTERFACE_DATA structure as a parameter verifies whether the <b>cbSize</b> member of the supplied structure is equal to the size, in bytes, of the structure. If the <b>cbSize</b> member is not set correctly, the function will fail and set an error code of ERROR_INVALID_USER_BUFFER.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff552343">SP_DEVICE_INTERFACE_DETAIL_DATA</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550965">SetupDiCreateDeviceInterface</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551015">SetupDiEnumDeviceInterfaces</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551108">SetupDiGetDeviceInterfaceAlias</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552074">SetupDiOpenDeviceInterface</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552149">SetupDiSetDeviceInterfaceDefault</a>
 

 
