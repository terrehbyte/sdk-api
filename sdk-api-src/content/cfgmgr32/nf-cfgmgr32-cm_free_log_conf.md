---
UID: NF:cfgmgr32.CM_Free_Log_Conf
title: CM_Free_Log_Conf function
author: windows-driver-content
description: The CM_Free_Log_Conf function removes a logical configuration and all associated resource descriptors from the local machine.
old-location: devinst\cm_free_log_conf.htm
old-project: devinst
ms.assetid: 89d8e5ed-751c-4f85-8669-a33c6228fe22
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Free_Log_Conf, CM_Free_Log_Conf function [Device and Driver Installation], cfgmgr32/CM_Free_Log_Conf, cfgmgrfn_68a9c019-f83c-4453-a988-3e9b1b33dd5f.xml, devinst.cm_free_log_conf
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Desktop
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
-	Cfgmgr32.dll
api_name:
-	CM_Free_Log_Conf
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
---

# CM_Free_Log_Conf function


## -description


The <b>CM_Free_Log_Conf</b> function removes a <a href="https://msdn.microsoft.com/c7a6997b-34f9-4dd9-b384-2321a8b5ce54">logical configuration</a> and all associated <a href="https://msdn.microsoft.com/004698f5-cb0e-4995-a19c-7075aa226000">resource descriptors</a> from the local machine.


## -parameters




### -param lcLogConfToBeFreed [in]

Caller-supplied handle to a logical configuration. This handle must have been previously obtained by calling one of the following functions:


<a href="https://msdn.microsoft.com/library/windows/hardware/ff537921">CM_Add_Empty_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff537926">CM_Add_Empty_Log_Conf_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538522">CM_Get_First_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538529">CM_Get_First_Log_Conf_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538591">CM_Get_Next_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538598">CM_Get_Next_Log_Conf_Ex</a>



### -param ulFlags [in]

Not used, must be zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.

<div class="alert"><b>Note</b>  Starting with Windows 8, <b>CM_Free_Log_Conf</b> returns CR_CALL_NOT_IMPLEMENTED when used in a Wow64 scenario. To request information about the hardware resources on a local machine it is necessary implement an architecture-native version of the application using the hardware resource APIs. For example: An AMD64 application for AMD64 systems.</div>
<div> </div>



## -remarks



Calling <b>CM_Free_Log_Conf</b> can cause the handles returned by <a href="https://msdn.microsoft.com/library/windows/hardware/ff538522">CM_Get_First_Log_Conf</a> and <a href="https://msdn.microsoft.com/library/windows/hardware/ff538591">CM_Get_Next_Log_Conf</a> to become invalid. Thus if you want to obtain logical configurations after calling <b>CM_Free_Log_Conf</b>, your code must call <b>CM_Get_First_Log_Conf</b> again and start at the first configuration.

Note that calling <b>CM_Free_Log_Conf</b> frees the configuration, but not the configuration's handle. To free the handle, call <b>CM_Free_Log_Conf_Handle</b>.

Callers of this function must have <b>SeLoadDriverPrivilege</b>. (Privileges are described in the Microsoft Windows SDK documentation.)




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538043">CM_Free_Log_Conf_Ex</a>
 

 
