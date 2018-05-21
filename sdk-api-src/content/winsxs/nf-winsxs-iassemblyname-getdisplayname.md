---
UID: NF:winsxs.IAssemblyName.GetDisplayName
title: IAssemblyName::GetDisplayName
author: windows-driver-content
description: The GetDisplayName method gets a string representation of the side-by-side assembly name.
old-location: setup\iassemblyname_getdisplayname.htm
old-project: SbsCs
ms.assetid: d2d74d67-a893-4f2f-8161-80bf3d5cbedb
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetDisplayName, GetDisplayName method [Side-by-side Assemblies], GetDisplayName method [Side-by-side Assemblies],IAssemblyName interface, IAssemblyName interface [Side-by-side Assemblies],GetDisplayName method, IAssemblyName.GetDisplayName, IAssemblyName::GetDisplayName, setup.iassemblyname_getdisplayname, winsxs/IAssemblyName::GetDisplayName
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: winsxs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: CREATE_ASM_NAME_OBJ_FLAGS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	sxs.dll
api_name:
-	IAssemblyName.GetDisplayName
product: Windows
targetos: Windows
req.lib: 
req.dll: Sxs.dll
req.irql: 
req.product: Windows XP Professional x64 Edition or 64-bit editions of     Windows Server 2003
---

# IAssemblyName::GetDisplayName


## -description


The <b>GetDisplayName</b> method gets a string representation of the side-by-side assembly name.


## -parameters




### -param szDisplayName [out]

A pointer to a buffer that receives the string value that contains the assembly name.


### -param pccDisplayName [in, out]

When calling this method, set this parameter to the size of the buffer specified by <b>szDisplayName</b>. Specify the size in characters and include the null terminator. When the method returns, the value of <i>pccDisplayName</i> is the size of the name returned.


### -param dwDisplayFlags [in]

One or more of the options of the <a href="https://msdn.microsoft.com/8f4c00b9-2684-44eb-9a68-bef6da87c396">ASM_DISPLAY_FLAGS</a> enumeration to specify which portions of the assembly's name to include in the string representation of the assembly name. The default for <i>dwDisplayFlags</i> is 0, which returns all portions of the assembly's display name.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>S_OK</dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>S_FALSE</dt>
</dl>
</td>
<td width="60%">
The method did not succeed.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/304b8fb3-5d17-4af0-b070-450a40dc5cc9">IAssemblyName</a>
 

 
