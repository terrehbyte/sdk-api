---
UID: NF:winsxs.IAssemblyName.GetName
title: IAssemblyName::GetName
author: windows-driver-content
description: The GetName method returns the name portion of the assembly name.
old-location: setup\iassemblyname_getname.htm
old-project: SbsCs
ms.assetid: b27ebe4e-02b6-473f-a8cb-c68a3e65e493
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetName, GetName method [Side-by-side Assemblies], GetName method [Side-by-side Assemblies],IAssemblyName interface, IAssemblyName interface [Side-by-side Assemblies],GetName method, IAssemblyName.GetName, IAssemblyName::GetName, setup.iassemblyname_getname, winsxs/IAssemblyName::GetName
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
-	IAssemblyName.GetName
product: Windows
targetos: Windows
req.lib: 
req.dll: Sxs.dll
req.irql: 
req.product: Windows XP Professional x64 Edition or 64-bit editions of     Windows Server 2003
---

# IAssemblyName::GetName


## -description


The <b>GetName</b> method returns the name portion of the assembly name.


## -parameters




### -param lpcwBuffer [in, out]

When calling this method, set this parameter to the size of the buffer specified by <i>pwzName</i>. The specify the size in characters and include the null terminator. When the method returns, the value of <i>lpcwBuffer</i> is the size of the name returned. 


### -param pwzName [out]

Pointer to the string value that receives  the name.


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
 




## -remarks



This method is equivalent to using the <a href="https://msdn.microsoft.com/0526fac9-1a3f-403b-b886-a7f833913e18">GetProperty</a> method with the <i>PropertyId</i> set to the <b>ASM_NAME_NAME</b> option of <a href="https://msdn.microsoft.com/5e13e90e-68b0-4842-97de-4f179d4c9ad7">ASM_NAME</a>. In case ASM_NAME_NAME is not set, the size of the buffer returned by <i>lpcwBuffer</i> is  0, and the content of <i>pwzName</i> is undefined.




## -see-also




<a href="https://msdn.microsoft.com/304b8fb3-5d17-4af0-b070-450a40dc5cc9">IAssemblyName</a>
 

 
