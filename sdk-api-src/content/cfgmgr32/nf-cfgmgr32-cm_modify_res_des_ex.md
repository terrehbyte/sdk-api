---
UID: NF:cfgmgr32.CM_Modify_Res_Des_Ex
title: CM_Modify_Res_Des_Ex function
author: windows-driver-content
description: The CM_Modify_Res_Des_Ex function modifies a specified resource descriptor on a local or a remote machine.
old-location: devinst\cm_modify_res_des_ex.htm
old-project: devinst
ms.assetid: 6bb4af46-995e-4487-9c5f-89c72abb0ec5
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Modify_Res_Des_Ex, CM_Modify_Res_Des_Ex function [Device and Driver Installation], cfgmgr32/CM_Modify_Res_Des_Ex, cfgmgrfn_62acb8c0-8f2c-4475-8f66-deed331699ba.xml, devinst.cm_modify_res_des_ex
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
-	CM_Modify_Res_Des_Ex
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
---

# CM_Modify_Res_Des_Ex function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/ff538763">CM_Modify_Res_Des</a> instead.]

The <b>CM_Modify_Res_Des_Ex</b> function modifies a specified resource descriptor on a local or a remote machine.


## -parameters




### -param prdResDes [out]

Pointer to a location to receive a handle to the modified resource descriptor.


### -param rdResDes [in]

Caller-supplied handle to the resource descriptor to be modified. This handle must have been previously obtained by calling one of the following functions:


<a href="https://msdn.microsoft.com/library/windows/hardware/ff537939">CM_Add_Res_Des</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff537941">CM_Add_Res_Des_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538600">CM_Get_Next_Res_Des</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538603">CM_Get_Next_Res_Des_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538763">CM_Modify_Res_Des</a>


<b>CM_Modify_Res_Des_Ex</b>


### -param ResourceID [in]

Caller-supplied resource type identifier. This must be one of the <b>ResType_</b>-prefixed constants defined in <i>Cfgmgr32.h</i>.


### -param ResourceData [in]

Caller-supplied pointer to a resource descriptor, which can be one of the structures listed under the <a href="https://msdn.microsoft.com/library/windows/hardware/ff537941">CM_Add_Res_Des_Ex</a> function's description of <i>ResourceData</i>.


### -param ResourceLen [in]

Caller-supplied length of the structure pointed to by <i>ResourceData</i>.


### -param ulFlags [in]

Not used, must be zero.


### -param hMachine [in, optional]

Caller-supplied machine handle, obtained from a previous call to <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.

<div class="alert"><b>Note</b>  Starting with Windows 8, <b>CM_Modify_Res_Des_Ex</b> returns CR_CALL_NOT_IMPLEMENTED when used in a Wow64 scenario. To request information about the hardware resources on a local machine it is necessary implement an architecture-native version of the application using the hardware resource APIs. For example: An AMD64 application for AMD64 systems.</div>
<div> </div>



## -remarks



The caller-supplied resource descriptor data replaces the existing data. The values specified for <i>ResourceID</i> and <i>ResourceLen</i> do not have to match the existing resource descriptor.

If the value specified for <i>ResourceID</i> is <b>ResType_ClassSpecific</b>, then the specified resource descriptor must be the last one associated with the logical configuration.

Callers of <b>CM_Modify_Res_Des_Ex</b> must call <a href="https://msdn.microsoft.com/library/windows/hardware/ff538067">CM_Free_Res_Des_Handle</a> to deallocate the resource descriptor handle, after it is no longer needed.

Callers of this function must have <b>SeLoadDriverPrivilege</b>. (Privileges are described in the Microsoft Windows SDK documentation.)

 Functionality to access remote machines has been removed in Windows 8 and Windows Server 2012 and later operating systems thus you cannot access remote machines when running on these versions of Windows.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538763">CM_Modify_Res_Des</a>
 

 
