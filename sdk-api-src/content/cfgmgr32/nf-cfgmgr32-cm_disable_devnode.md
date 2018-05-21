---
UID: NF:cfgmgr32.CM_Disable_DevNode
title: CM_Disable_DevNode function
author: windows-driver-content
description: The CM_Disable_DevNode function disables a device.
old-location: devinst\cm_disable_devnode.htm
old-project: devinst
ms.assetid: 6013fec3-1fb3-4956-982d-5841518f5d31
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Disable_DevNode, CM_Disable_DevNode function [Device and Driver Installation], cfgmgr32/CM_Disable_DevNode, cfgmgrfn_3a8b48b2-fb94-421c-9ec4-2e88997eb9b5.xml, devinst.cm_disable_devnode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Universal
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
-	API-MS-Win-devices-config-l1-1-0.dll
-	API-MS-Win-devices-config-l1-1-1.dll
api_name:
-	CM_Disable_DevNode
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib; OneCoreUAP.lib on Windows 10
req.dll: CfgMgr32.dll
req.irql: 
---

# CM_Disable_DevNode function


## -description


The <b>CM_Disable_DevNode</b> function disables a device.


## -parameters




### -param dnDevInst [in]

Device instance handle that is bound to the local machine.


### -param ulFlags [in]

Disable flags:





#### CM_DISABLE_UI_NOT_OK

Do not display any interface to the user if the attempt to disable the device fails.



#### CM_DISABLE_PERSIST

Disables the device across reboots.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



By default, <b>CM_Disable_DevNode</b> disables a device at one time, but after reboot the device is enabled again. Starting in Windows 10, you can specify the <b>CM_DISABLE_PERSIST</b> flag to disable the device across reboots.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538015">CM_Enable_DevNode</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543712">DIF_PROPERTYCHANGE</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a>
 

 
