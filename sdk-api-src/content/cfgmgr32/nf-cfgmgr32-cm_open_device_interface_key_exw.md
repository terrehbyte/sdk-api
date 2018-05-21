---
UID: NF:cfgmgr32.CM_Open_Device_Interface_Key_ExW
title: CM_Open_Device_Interface_Key_ExW function
author: windows-driver-content
description: The CM_Open_Device_Interface_Key_ExW function opens the registry subkey that is used by applications and drivers to store information that is specific to a device interface.
old-location: devinst\cm_open_device_interface_key_exw.htm
old-project: devinst
ms.assetid: 71F8EF83-4DEC-4BDC-BBCE-4F7C232F1768
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Open_Device_Interface_KeyA, CM_Open_Device_Interface_KeyW, CM_Open_Device_Interface_Key_ExW, CM_Open_Device_Interface_Key_ExW function [Device and Driver Installation], cfgmgr32/CM_Open_Device_Interface_KeyA, cfgmgr32/CM_Open_Device_Interface_KeyW, cfgmgr32/CM_Open_Device_Interface_Key_ExW, devinst.cm_open_device_interface_key_exw
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
req.unicode-ansi: CM_Open_Device_Interface_KeyW (Unicode) and CM_Open_Device_Interface_KeyA (ANSI)
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
-	CM_Open_Device_Interface_Key_ExW
-	CM_Open_Device_Interface_KeyA
-	CM_Open_Device_Interface_KeyW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Open_Device_Interface_Key_ExW function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/hh780223">CM_Open_Device_Interface_Key</a> instead.]

The <b>CM_Open_Device_Interface_Key_ExW</b> function opens the registry subkey that is used by applications and drivers to store information that is specific to a device interface.


## -parameters




### -param pszDeviceInterface [in]

Pointer to a string that identifies the device interface instance to open the registry subkey for.


### -param samDesired [in]

The requested registry security access to the registry subkey.


### -param Disposition [in]

Specifies how the registry key is to be opened. May be one of the following values:





#### RegDisposition_OpenAlways

Open the key if it exists. Otherwise, create the key.



#### RegDisposition_OpenExisting

Open the key only if it exists.


### -param phkDeviceInterface [out]

Pointer to an HKEY that will receive the opened key upon success.


### -param ulFlags [in]

Reserved. Must be set to zero.


### -param hMachine [in, optional]

Caller-supplied machine handle, obtained from a previous call to <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



Close the handle returned from this function by calling <b>RegCloseKey</b>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552075">SetupDiOpenDeviceInterfaceRegKey</a>
 

 
