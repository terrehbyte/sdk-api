---
UID: NF:tapi3if.ITBasicAudioTerminal.put_Volume
title: ITBasicAudioTerminal::put_Volume
author: windows-driver-content
description: The put_Volume method sets the volume.
old-location: tapi3\itbasicaudioterminal_put_volume.htm
old-project: Tapi
ms.assetid: 6c611505-74b4-48fa-bb36-ec765cb24f96
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITBasicAudioTerminal interface [TAPI 2.2],put_Volume method, ITBasicAudioTerminal.put_Volume, ITBasicAudioTerminal::put_Volume, _tapi3_itbasicaudioterminal_put_volume, put_Volume, put_Volume method [TAPI 2.2], put_Volume method [TAPI 2.2],ITBasicAudioTerminal interface, tapi3.itbasicaudioterminal_put_volume, tapi3if/ITBasicAudioTerminal::put_Volume
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
-	ITBasicAudioTerminal.put_Volume
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITBasicAudioTerminal::put_Volume


## -description


The 
<b>put_Volume</b> method sets the volume.


## -parameters




### -param lVolume [in]

The volume property is a value between 0 and FFFF, representing a set of logarithmic steps. Not all devices support as many distinguishable steps.


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
<tr>
<td width="40%">
<dl>
<dt><b>TAPI_E_NOTERMINALSELECTED</b></dt>
</dl>
</td>
<td width="60%">
A terminal must be selected before the volume can be adjusted.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/3e676a16-f3ce-433c-9941-8cdccdb01efd">ITBasicAudioTerminal</a>



<a href="https://msdn.microsoft.com/0d96f229-76c0-46a3-bc4b-6f558b9956c6">Terminal Object</a>



<a href="https://msdn.microsoft.com/2d3a64fa-41b6-44c4-a67e-08113e771cc7">get_Volume</a>
 

 
