---
UID: NF:tapi3if.IEnumCallingCard.Clone
title: IEnumCallingCard::Clone
author: windows-driver-content
description: The Clone method creates another enumerator that contains the same enumeration state as the current one. This method is hidden from Visual Basic and scripting languages.
old-location: tapi3\ienumcallingcard_clone.htm
old-project: Tapi
ms.assetid: fb1a2ac3-12d1-42f0-9c73-c4d0d8a88700
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: Clone, Clone method [TAPI 2.2], Clone method [TAPI 2.2],IEnumCallingCard interface, IEnumCallingCard interface [TAPI 2.2],Clone method, IEnumCallingCard.Clone, IEnumCallingCard::Clone, _tapi3_ienumcallingcard_clone, tapi3.ienumcallingcard_clone, tapi3if/IEnumCallingCard::Clone
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
-	IEnumCallingCard.Clone
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumCallingCard::Clone


## -description


The 
<b>Clone</b> method creates another enumerator that contains the same enumeration state as the current one. This method is hidden from Visual Basic and scripting languages.


## -parameters




### -param ppEnum [out]

Pointer to new 
<a href="https://msdn.microsoft.com/d2eed88b-9a01-4205-a35d-92a24e07a1e2">IEnumCallingCard</a> interface.


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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppEnum</i> parameter not a valid pointer.

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
<tr>
<td width="40%">
<dl>
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
Failed for unknown reasons.

</td>
</tr>
</table>
 




## -remarks



TAPI calls the <a href="_com_iunknown_addref">AddRef</a> method on the 
<a href="https://msdn.microsoft.com/d2eed88b-9a01-4205-a35d-92a24e07a1e2">IEnumCallingCard</a> interface returned by <b>IEnumCallingCard::Clone</b>. The application must call <a href="_com_iunknown_release">Release</a> on the 
<b>IEnumCallingCard</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal Object</a>
 

 
