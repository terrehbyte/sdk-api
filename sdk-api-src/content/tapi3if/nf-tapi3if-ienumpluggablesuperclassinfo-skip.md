---
UID: NF:tapi3if.IEnumPluggableSuperclassInfo.Skip
title: IEnumPluggableSuperclassInfo::Skip
author: windows-driver-content
description: The Skip method skips over the next specified number of elements in the enumeration sequence. This method is hidden from Visual Basic and scripting languages.
old-location: tapi3\ienumpluggablesuperclassinfo_skip.htm
old-project: Tapi
ms.assetid: ad23eeb8-295c-43d0-af50-fa5fef0f295b
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: IEnumPluggableSuperclassInfo interface [TAPI 2.2],Skip method, IEnumPluggableSuperclassInfo.Skip, IEnumPluggableSuperclassInfo::Skip, Skip, Skip method [TAPI 2.2], Skip method [TAPI 2.2],IEnumPluggableSuperclassInfo interface, _tapi3_ienumpluggablesuperclassinfo_skip, tapi3.ienumpluggablesuperclassinfo_skip, tapi3if/IEnumPluggableSuperclassInfo::Skip
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
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
req.typenames: TERMINAL_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Tapi3.dll
api_name:
-	IEnumPluggableSuperclassInfo.Skip
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumPluggableSuperclassInfo::Skip


## -description


The 
<b>Skip</b> method skips over the next specified number of elements in the enumeration sequence. This method is hidden from Visual Basic and scripting languages.


## -parameters




### -param celt [in]

Number of elements to skip.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Number of elements skipped was <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
Number of elements skipped was not <i>celt</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/80b84976-4256-47d2-a965-3ebe89a3821a">IEnumPluggableSuperclassInfo</a>
 

 
