---
UID: NF:cfgmgr32.CM_Uninstall_DevNode
title: CM_Uninstall_DevNode function
author: windows-driver-content
description: The CM_Uninstall_DevNode function removes all persistent state associated with a device instance.
old-location: devinst\cm_uninstall_devnode.htm
old-project: devinst
ms.assetid: e472e642-cf0d-4c88-907f-5cfb08fb4e76
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Uninstall_DevNode, CM_Uninstall_DevNode function [Device and Driver Installation], cfgmgr32/CM_Uninstall_DevNode, cfgmgrfn_a3aadd47-2a1b-4123-823f-7d7cb988812e.xml, devinst.cm_uninstall_devnode
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
-	CM_Uninstall_DevNode
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib; OneCoreUAP.lib on Windows 10
req.dll: CfgMgr32.dll
req.irql: 
---

# CM_Uninstall_DevNode function


## -description


The <b>CM_Uninstall_DevNode</b> function removes all persistent state associated with a device instance.


## -parameters




### -param dnDevInst [in]

Device instance handle that is bound to the local machine.


### -param ulFlags [in]

Reserved. Must be set to zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



This function uninstalls the device without sending an <b>IRP_MN_QUERY_REMOVE_DEVICE</b> request or calling class installers or co-installers.       If your application will run only on a <a href="https://docs.microsoft.com/windows-hardware/drivers/develop/windows-10-editions-for-universal-drivers">Target Platform</a> of Desktop, instead of calling <b>CM_Uninstall_DevNode</b>, the application should uninstall the device by calling <a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a> with the <a href="https://msdn.microsoft.com/library/windows/hardware/ff543717">DIF_REMOVE</a> code, or by calling <a href="https://msdn.microsoft.com/library/windows/hardware/ff544754">DiUninstallDevice</a>.

Use the following sequence to call this function:

<ol>
<li>Check if <a href="https://msdn.microsoft.com/library/windows/hardware/ff538514">CM_Get_DevNode_Status</a> returns success.  This means that the device is present.</li>
<li>If the device is present, call <a href="https://msdn.microsoft.com/library/windows/hardware/ff539722">CM_Query_And_Remove_SubTree</a>.</li>
<li>Call <b>CM_Uninstall_DevNode</b>.</li>
</ol>



## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a>
 

 
