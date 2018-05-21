---
UID: NN:tapi3if.IEnumStream
title: IEnumStream
author: windows-driver-content
description: The IEnumStream interface provides COM-standard enumeration methods for the ITStream interface. The ITStreamControl::EnumerateStreams and ITParticipant::EnumerateStreams methods return a pointer to IEnumStream.
old-location: tapi3\ienumstream.htm
old-project: Tapi
ms.assetid: 52e8c040-8bc5-4c9c-a697-ec05164adea2
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: IEnumStream, IEnumStream interface [TAPI 2.2], IEnumStream interface [TAPI 2.2],described, _tapi3_ienumstream, tapi3.ienumstream, tapi3if/IEnumStream
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
-	tapi3if.h
api_name:
-	IEnumStream
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumStream interface


## -description


The 
<b>IEnumStream</b> interface provides COM-standard enumeration methods for the 
<a href="https://msdn.microsoft.com/74a385c8-0c36-4cf0-8983-5ffd7b0e5c4a">ITStream</a> interface. The 
<a href="https://msdn.microsoft.com/de018f3e-d3b9-4093-a2b5-4929ac4d1d2a">ITStreamControl::EnumerateStreams</a> and 
<a href="https://msdn.microsoft.com/de018f3e-d3b9-4093-a2b5-4929ac4d1d2a">ITParticipant::EnumerateStreams</a> methods return a pointer to 
<b>IEnumStream</b>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEnumStream</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IEnumStream</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEnumStream</b> interface has these methods.
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
Resets to beginning of enumeration sequence.

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


## -see-also




<a href="https://msdn.microsoft.com/74a385c8-0c36-4cf0-8983-5ffd7b0e5c4a">ITStream</a>



<a href="https://msdn.microsoft.com/53b7bcbd-571a-44da-a6db-10d4c3e5d30a">Media Service Provider Interface (MSPI)</a>
 

 
