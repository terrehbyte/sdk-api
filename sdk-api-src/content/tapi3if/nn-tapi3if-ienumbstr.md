---
UID: NN:tapi3if.IEnumBstr
title: IEnumBstr
author: windows-driver-content
description: The IEnumBstr interface provides COM-standard methods to enumerate BSTR strings.
old-location: tapi3\ienumbstr.htm
old-project: Tapi
ms.assetid: 0e87ec06-7f3a-410c-9d54-7a67991e089c
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: IEnumBstr, IEnumBstr interface [TAPI 2.2], IEnumBstr interface [TAPI 2.2],described, _tapi3_ienumbstr, tapi3.ienumbstr, tapi3if/IEnumBstr
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
-	IEnumBstr
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumBstr interface


## -description


The 
<b>IEnumBstr</b> interface provides COM-standard methods to enumerate <b>BSTR</b> strings. The following methods return a pointer to this interface:
<ul>
<li>
<a href="https://msdn.microsoft.com/34a967ba-7d1f-4841-95be-9e83f927379b">ITAddressCapabilities::EnumerateCallTreatments</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b7a3eb72-6c9f-4164-a082-8b0951733dcb">ITAddressCapabilities::EnumerateCompletionMessages</a>
</li>
<li>
<a href="https://msdn.microsoft.com/33cc965f-0603-40b0-95bb-9b16025dd2b6">ITAddressCapabilities::EnumerateDeviceClasses</a>
</li>
<li>
<a href="https://msdn.microsoft.com/edbfe386-9b3d-4160-916e-6c9ea640cfbc">IMcastLeaseInfo::EnumerateAddresses</a>
</li>
</ul>The 
<b>IEnumBstr</b> interface is hidden from Visual Basic and scripting languages.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumBstr</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumBstr</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumBstr</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/dn938510">Clone</a>
</td>
<td align="left" width="63%">
Creates another enumerator that contains the same enumeration state as the current one.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/dn926903">Next</a>
</td>
<td align="left" width="63%">
Gets the next specified number of elements in the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/dn926942">Reset</a>
</td>
<td align="left" width="63%">
Resets to the beginning of the enumeration sequence.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/dn926952">Skip</a>
</td>
<td align="left" width="63%">
Skips over the next specified number of elements in the enumeration sequence.

</td>
</tr>
</table> 
