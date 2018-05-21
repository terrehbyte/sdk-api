---
UID: NF:tapi3if.IEnumTerminal.Reset
title: IEnumTerminal::Reset
author: windows-driver-content
description: The Reset method resets to the beginning of the enumeration sequence. This method is hidden from Visual Basic and scripting languages.
old-location: tapi3\ienumterminal_reset.htm
old-project: Tapi
ms.assetid: 4f8e9b85-abdb-41fb-8e7d-fbcde92f4458
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: IEnumTerminal interface [TAPI 2.2],Reset method, IEnumTerminal.Reset, IEnumTerminal::Reset, Reset, Reset method [TAPI 2.2], Reset method [TAPI 2.2],IEnumTerminal interface, _tapi3_ienumterminal_reset, tapi3.ienumterminal_reset, tapi3if/IEnumTerminal::Reset
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
-	IEnumTerminal.Reset
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumTerminal::Reset


## -description


The 
<b>Reset</b> method resets to the beginning of the enumeration sequence. This method is hidden from Visual Basic and scripting languages.


## -parameters






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
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal Object</a>
 

 
