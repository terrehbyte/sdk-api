---
UID: NF:winsxs.IAssemblyName.SetProperty
title: IAssemblyName::SetProperty
author: windows-driver-content
description: The SetProperty method adds a name-value pair to the side-by-side assembly name. This method can change or delete the value of an existing name-value pair.
old-location: setup\iassemblyname_setproperty.htm
old-project: SbsCs
ms.assetid: 057bc5b3-008b-495b-b96c-2c0dcc43f1a4
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IAssemblyName interface [Side-by-side Assemblies],SetProperty method, IAssemblyName.SetProperty, IAssemblyName::SetProperty, SetProperty, SetProperty method [Side-by-side Assemblies], SetProperty method [Side-by-side Assemblies],IAssemblyName interface, setup.iassemblyname_setproperty, winsxs/IAssemblyName::SetProperty
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
-	IAssemblyName.SetProperty
product: Windows
targetos: Windows
req.lib: 
req.dll: Sxs.dll
req.irql: 
req.product: Windows XP Professional x64 Edition or 64-bit editions of     Windows Server 2003
---

# IAssemblyName::SetProperty


## -description


The <b>SetProperty</b> method adds a name-value pair to the side-by-side assembly name. This method can change or delete the value of an existing name-value pair.


## -parameters




### -param PropertyId [in]

A property ID that represents the name-value pair. Valid property IDs are <a href="https://msdn.microsoft.com/5e13e90e-68b0-4842-97de-4f179d4c9ad7">ASM_NAME</a> enumeration values.


### -param pvProperty [in]

A pointer to a buffer that contains the value of the name-value pair.


### -param cbProperty [in, optional]

The size in bytes of the buffer specified by <i>pvProperty</i>. Set the value of this parameter to zero to remove the name-value pair from the assembly name.


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
<tr>
<td width="40%">
<dl>
<dt>E_UNEXPECTED</dt>
</dl>
</td>
<td width="60%">
The method did not succeed. The <a href="https://msdn.microsoft.com/057bc5b3-008b-495b-b96c-2c0dcc43f1a4">SetProperty</a> method was called after the <a href="https://msdn.microsoft.com/9930826e-3082-4ad3-991e-13cf426983a4">Finalize</a> method.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/304b8fb3-5d17-4af0-b070-450a40dc5cc9">IAssemblyName</a>
 

 
