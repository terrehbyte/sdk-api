---
UID: NF:tapi3if.ITScriptableAudioFormat.get_AvgBytesPerSec
title: ITScriptableAudioFormat::get_AvgBytesPerSec
author: windows-driver-content
description: The get_AvgBytesPerSec method returns the value for the nAvgBytesPerSec member in the WAVEFORMATEX structure.
old-location: tapi3\itscriptableaudioformat_get_avgbytespersec.htm
old-project: Tapi
ms.assetid: fe54e1a5-ff8f-486d-90ba-3c7fc595ec1d
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITScriptableAudioFormat interface [TAPI 2.2],get_AvgBytesPerSec method, ITScriptableAudioFormat.get_AvgBytesPerSec, ITScriptableAudioFormat::get_AvgBytesPerSec, _tapi3_itscriptableaudioformat_get_avgbytespersec, get_AvgBytesPerSec, get_AvgBytesPerSec method [TAPI 2.2], get_AvgBytesPerSec method [TAPI 2.2],ITScriptableAudioFormat interface, tapi3.itscriptableaudioformat_get_avgbytespersec, tapi3if/ITScriptableAudioFormat::get_AvgBytesPerSec
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
-	ITScriptableAudioFormat.get_AvgBytesPerSec
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITScriptableAudioFormat::get_AvgBytesPerSec


## -description


The 
<b>get_AvgBytesPerSec</b> method returns the value for the <b>nAvgBytesPerSec</b> member in the 
<a href="https://msdn.microsoft.com/library/windows/hardware/ff538799">WAVEFORMATEX</a> structure.


## -parameters




### -param pVal [out]

Pointer to the value for the <b>nAvgBytesPerSec</b> member in the 
<a href="https://msdn.microsoft.com/library/windows/hardware/ff538799">WAVEFORMATEX</a> structure.


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
Method succeeded

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>pVal</i> argument is not a valid pointer.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/6b5d069a-044f-4bd4-b661-6100a2607107">ITScriptableAudioFormat</a>



<a href="https://msdn.microsoft.com/ca1b67b3-2dd0-47c1-9e91-ae94b6d78cc4">put_AvgBytesPerSec</a>
 

 
