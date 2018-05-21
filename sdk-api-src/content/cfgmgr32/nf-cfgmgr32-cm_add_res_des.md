---
UID: NF:cfgmgr32.CM_Add_Res_Des
title: CM_Add_Res_Des function
author: windows-driver-content
description: The CM_Add_Res_Des function adds a resource descriptor to a logical configuration.
old-location: devinst\cm_add_res_des.htm
old-project: devinst
ms.assetid: 0097b53a-c1c8-4e76-beef-812a953073b6
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Add_Res_Des, CM_Add_Res_Des function [Device and Driver Installation], cfgmgr32/CM_Add_Res_Des, cfgmgrfn_86ee6b93-0cdd-4f18-87c2-8c8d0c33d39f.xml, devinst.cm_add_res_des
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
-	CM_Add_Res_Des
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
---

# CM_Add_Res_Des function


## -description


The <b>CM_Add_Res_Des</b> function adds a <a href="https://msdn.microsoft.com/004698f5-cb0e-4995-a19c-7075aa226000">resource descriptor</a> to a <a href="https://msdn.microsoft.com/c7a6997b-34f9-4dd9-b384-2321a8b5ce54">logical configuration</a>.


## -parameters




### -param prdResDes [out, optional]

Pointer to a location to receive a handle to the new resource descriptor.


### -param lcLogConf [in]

Caller-supplied handle to the logical configuration to which the resource descriptor should be added. This handle must have been previously obtained by calling one of the following functions:


<a href="https://msdn.microsoft.com/library/windows/hardware/ff537921">CM_Add_Empty_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff537926">CM_Add_Empty_Log_Conf_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538522">CM_Get_First_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538529">CM_Get_First_Log_Conf_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538591">CM_Get_Next_Log_Conf</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538598">CM_Get_Next_Log_Conf_Ex</a>



### -param ResourceID [in]

Caller-supplied resource type identifier, which identifies the type of structure supplied by <i>ResourceData</i>. This must be one of the <b>ResType_</b>-prefixed constants defined in <i>Cfgmgr32.h</i>.


### -param ResourceData [in]

Caller-supplied pointer to one of the resource structures listed in the following table.

<table>
<tr>
<th><i>ResourceID </i>Parameter</th>
<th>Resource Structure</th>
</tr>
<tr>
<td>
<b>ResType_BusNumber</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff537838">BUSNUMBER_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_ClassSpecific</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff540237">CS_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_DevicePrivate</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff543542">DEVPRIVATE_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_DMA</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff544764">DMA_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_IO</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff548201">IO_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_IRQ</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff548229">IRQ_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_Mem</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff548724">MEM_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_MfCardConfig</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff549273">MFCARD_RESOURCE</a>


</td>
</tr>
<tr>
<td>
<b>ResType_PcCardConfig</b>

</td>
<td>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff549665">PCCARD_RESOURCE</a>


</td>
</tr>
</table>
 


### -param ResourceLen [in]

Caller-supplied length of the structure pointed to by <i>ResourceData</i>.


### -param ulFlags [in]

Not used, must be zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.

<div class="alert"><b>Note</b>  Starting with Windows 8,  <b>CM_Add_Res_Des</b> returns CR_CALL_NOT_IMPLEMENTED when used in a Wow64 scenario. To request information about the hardware resources on a local machine it is necessary implement an architecture-native version of the application using the hardware resource APIs. For example: An AMD64 application for AMD64 systems.</div>
<div> </div>



## -remarks



Callers of <b>CM_Add_Res_Des</b> must call <a href="https://msdn.microsoft.com/library/windows/hardware/ff538067">CM_Free_Res_Des_Handle</a> to deallocate the resource descriptor handle, after it is no longer needed.

Callers of this function must have <b>SeLoadDriverPrivilege</b>. (Privileges are described in the Microsoft Windows SDK documentation.)




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537941">CM_Add_Res_Des_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538067">CM_Free_Res_Des_Handle</a>
 

 
