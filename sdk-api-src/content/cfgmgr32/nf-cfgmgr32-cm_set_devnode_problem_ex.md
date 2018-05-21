---
UID: NF:cfgmgr32.CM_Set_DevNode_Problem_Ex
title: CM_Set_DevNode_Problem_Ex function
author: windows-driver-content
description: The CM_Set_DevNode_Problem_Ex function sets a problem code for a device that is installed in a local or a remote machine.
old-location: devinst\cm_set_devnode_problem_ex.htm
old-project: devinst
ms.assetid: 2e3e2c3a-c507-4cc8-bc2c-823d0b597704
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Set_DevNode_Problem_Ex, CM_Set_DevNode_Problem_Ex function [Device and Driver Installation], cfgmgr32/CM_Set_DevNode_Problem_Ex, cfgmgrfn_a2853e6a-afab-4725-bbe3-520605d515f0.xml, devinst.cm_set_devnode_problem_ex
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
-	CM_Set_DevNode_Problem_Ex
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
---

# CM_Set_DevNode_Problem_Ex function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated.  Please use <a href="https://msdn.microsoft.com/library/windows/hardware/ff539837">CM_Set_DevNode_Problem</a> instead.]

The <b>CM_Set_DevNode_Problem_Ex</b> function sets a problem code for a device that is installed in a local or a remote machine.


## -parameters




### -param dnDevInst [in]

Caller-supplied device instance handle that is bound to the machine handle supplied by <i>hMachine</i>.


### -param ulProblem [in]

Supplies a problem code, which is zero or one of the CM_PROB_Xxx flags that are described in <a href="devinst.device_manager_error_messages">Device Manager Error Messages</a>. A value of zero indicates that a problem code is not set for the device. 


### -param ulFlags [in]

Must be set to zero.


### -param hMachine [in, optional]

Caller-supplied machine handle to which the caller-supplied device instance handle is bound.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, the function returns one of the CR_-prefixed error codes that are defined in <i>Cfgmgr32.h</i>.




## -remarks



Use this function to set a problem code for a device that is installed in a local or a remote machine. You can also use the following functions to set a device's problem code and to obtain the problem code set for the device:

<ul>
<li>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff538514">CM_Get_DevNode_Status</a> returns the problem code set for a device installed in a local machine.

</li>
<li>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff538517">CM_Get_DevNode_Status_Ex</a> returns the problem code set for a device installed in a local or a remote machine.

</li>
<li>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff539837">CM_Set_DevNode_Problem</a> sets a problem code for a device installed in a local machine.

</li>
</ul>
For information about using device instance handles that are bound to a local or a remote machine, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff538076">CM_Get_Child_Ex</a>.

 Functionality to access remote machines has been removed in Windows 8 and Windows Server 2012 and later operating systems thus you cannot access remote machines when running on these versions of Windows.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538076">CM_Get_Child_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538514">CM_Get_DevNode_Status</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538517">CM_Get_DevNode_Status_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff539837">CM_Set_DevNode_Problem</a>
 

 
