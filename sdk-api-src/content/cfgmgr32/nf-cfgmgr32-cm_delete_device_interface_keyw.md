---
UID: NF:cfgmgr32.CM_Delete_Device_Interface_KeyW
title: CM_Delete_Device_Interface_KeyW function
author: windows-driver-content
description: The CM_Delete_Device_Interface_Key function deletes the registry subkey that is used by applications and drivers to store interface-specific information.
old-location: devinst\cm_delete_device_interface_key.htm
old-project: devinst
ms.assetid: 3DA5BD50-54AE-47A5-A99C-9E24CB2FA3D6
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Delete_Device_Interface_Key, CM_Delete_Device_Interface_Key function [Device and Driver Installation], CM_Delete_Device_Interface_KeyW, cfgmgr32/CM_Delete_Device_Interface_Key, cfgmgr32/CM_Delete_Device_Interface_KeyW, devinst.cm_delete_device_interface_key
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
req.unicode-ansi: CM_Delete_Device_Interface_KeyW (Unicode)
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
-	API-Ms-Win-Devices-Config-L1-1-0.dll
-	API-Ms-Win-Devices-Config-L1-1-1.dll
-	CfgMgr32.dll
api_name:
-	CM_Delete_Device_Interface_Key
-	CM_Delete_Device_Interface_KeyW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Delete_Device_Interface_KeyW function


## -description


The <b>CM_Delete_Device_Interface_Key</b> function deletes the registry subkey that is used by applications and drivers to store interface-specific information.


## -parameters




### -param pszDeviceInterface [in]

Pointer to a string that identifies the device interface instance of the registry subkey to delete.


### -param ulFlags [in]

Reserved. Must be set to zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/hh780223">CM_Open_Device_Interface_Key</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550986">SetupDiDeleteDeviceInterfaceRegKey</a>
 

 
