---
UID: NF:vdssys.GetVirtualDiskOperationProgress
title: GetVirtualDiskOperationProgress function
author: windows-sdk-content
description: Checks the progress of an asynchronous virtual hard disk (VHD) operation.
old-location: vhd\getvirtualdiskoperationprogress.htm
old-project: VStor
ms.assetid: 392a5258-306d-4c06-a632-85e6fc65ddc9
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: GetVirtualDiskOperationProgress, GetVirtualDiskOperationProgress function [VHD], vdssys/GetVirtualDiskOperationProgress, vhd.getvirtualdiskoperationprogress, virtdisk/GetVirtualDiskOperationProgress
ms.prod: windows
ms.technology: windows-sdk
ms.topic: function
req.header: vdssys.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: VIRTUAL_DISK_ACCESS_MASK
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	VirtDisk.dll
api_name:
-	GetVirtualDiskOperationProgress
product: Windows
targetos: Windows
req.lib: VirtDisk.lib
req.dll: VirtDisk.dll
req.irql: 
req.product: Windows UI
---

# GetVirtualDiskOperationProgress function


## -description


Checks the progress of an asynchronous virtual hard disk (VHD) operation.


## -parameters




### -param VirtualDiskHandle [in]

A valid handle to a virtual disk with a pending asynchronous operation.


### -param Overlapped [in]

A pointer to a valid <a href="https://msdn.microsoft.com/5037f6b9-e316-483b-a8e2-b58d2587ebd9">OVERLAPPED</a> structure. This 
     parameter must reference the same structure previously sent to the virtual disk operation being checked for 
     progress.


### -param Progress [out]

A pointer to a <a href="https://msdn.microsoft.com/834d7384-09fe-493e-8402-135c453a1ecf">VIRTUAL_DISK_PROGRESS</a> 
     structure that receives the current virtual disk operation progress.


## -returns



Status of the request.

If the function succeeds, the return value is <b>ERROR_SUCCESS</b> and the 
      <i>Progress</i> parameter will be populated with the current virtual disk operation 
      progress.

If the function fails, the return value is an error code and the value of the 
      <i>Progress</i> parameter is undefined. For more information, see 
      <a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System Error Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/c9531c07-ad55-42b6-8685-7f55a47e8485">About VHD</a>



<a href="https://msdn.microsoft.com/3b5d0da0-2b23-4b7c-b007-ed3fe030926c">VHD Reference</a>



<a href="https://msdn.microsoft.com/834d7384-09fe-493e-8402-135c453a1ecf">VIRTUAL_DISK_PROGRESS</a>
 

 
