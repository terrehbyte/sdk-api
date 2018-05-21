---
UID: NF:cfgmgr32.CM_Get_Parent
title: CM_Get_Parent function
author: windows-driver-content
description: The CM_Get_Parent function obtains a device instance handle to the parent node of a specified device node (devnode) in the local machine's device tree.
old-location: devinst\cm_get_parent.htm
old-project: devinst
ms.assetid: e9d1db59-e9fb-4704-81f6-86523397c114
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Get_Parent, CM_Get_Parent function [Device and Driver Installation], cfgmgr32/CM_Get_Parent, cfgmgrfn_fdd00a0a-e79d-469d-9a1a-852096d89a48.xml, devinst.cm_get_parent
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Universal
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
-	CM_Get_Parent
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib; OneCoreUAP.lib on Windows 10
req.dll: CfgMgr32.dll
req.irql: 
---

# CM_Get_Parent function


## -description


The <b>CM_Get_Parent</b> function obtains a device instance handle to the parent node of a specified device node (<a href="https://msdn.microsoft.com/86688b5d-575d-42e1-9158-7ffba1aaf1d3">devnode</a>) in the local machine's device tree.


## -parameters




### -param pdnDevInst [out]

Caller-supplied pointer to the device instance handle to the parent node that this function retrieves. The retrieved handle is bound to the local machine.


### -param dnDevInst [in]

Caller-supplied device instance handle that is bound to the local machine.


### -param ulFlags [in]

Not used, must be zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



For information about using a device instance handle that is bound to the local machine, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff538074">CM_Get_Child</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538074">CM_Get_Child</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538615">CM_Get_Parent_Ex</a>
 

 
