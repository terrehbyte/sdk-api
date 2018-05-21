---
UID: NS:cfgmgr32.PcCard_Des_s
title: PcCard_Des_s
author: windows-driver-content
description: The PCCARD_DES structure is used for specifying either a resource list or a resource requirements list that describes resource usage by a PC Card instance. For more information about resource lists and resource requirements lists, see Hardware Resources.
old-location: devinst\pccard_des.htm
old-project: devinst
ms.assetid: d1bf4d50-70e1-4eff-8973-0b83a31f55fc
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PPCCARD_DES, PCCARD_DES, PCCARD_DES structure [Device and Driver Installation], PPCCARD_DES, PPCCARD_DES structure pointer [Device and Driver Installation], PcCard_Des_s, cfgmgr32/PCCARD_DES, cfgmgr32/PPCCARD_DES, cfgmgrst_c82ff49b-4ae5-478d-a981-26d75408b157.xml, devinst.pccard_des"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
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
req.typenames: PCCARD_DES, *PPCCARD_DES
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	cfgmgr32.h
api_name:
-	PCCARD_DES
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# PcCard_Des_s structure


## -description


The PCCARD_DES structure is used for specifying either a resource list or a resource requirements list that describes resource usage by a PC Card instance. For more information about resource lists and resource requirements lists, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff547012">Hardware Resources</a>.


## -struct-fields




### -field PCD_Count

Must be 1.


### -field PCD_Type

<i>Not used.</i>


### -field PCD_Flags

One bit flag from <i>each</i> of the flag sets described in the following table.

<table>
<tr>
<th></th>
<th>Flag</th>
<th>Definition</th>
</tr>
<tr>
<td colspan="2">
<i>I/O Addressing Flags</i>

</td>
<td></td>
</tr>
<tr>
<td></td>
<td>
fPCD_IO_8

</td>
<td>
The device uses 8-bit I/O addressing.

</td>
</tr>
<tr>
<td></td>
<td>
fPCD_IO_16

</td>
<td>
The device uses 16-bit I/O addressing.

</td>
</tr>
<tr>
<td></td>
<td>
mPCD_IO_8_16

</td>
<td>
Bitmask for the bit within <b>PCD_Flags</b> that specifies 8-bit or 16-bit I/O addressing.

</td>
</tr>
<tr>
<td colspan="2">
<i>Memory Addressing Flags</i>

</td>
<td></td>
</tr>
<tr>
<td></td>
<td>
fPCD_MEM_8

</td>
<td>
The device uses 8-bit memory addressing.

</td>
</tr>
<tr>
<td></td>
<td>
fPCD_MEM_16

</td>
<td>
The device uses 16-bit memory addressing.

</td>
</tr>
<tr>
<td></td>
<td>
mPCD_MEM_8_16

</td>
<td>
Bitmask for the bit within <b>PCD_Flags</b> that specifies 8-bit or 16-bit memory addressing.

</td>
</tr>
</table>
 


### -field PCD_ConfigIndex

The 8-bit index value used to locate the device's configuration.


### -field PCD_Reserved

<i>Not used.</i>


### -field PCD_MemoryCardBase1

<i>Optional</i>, card base address of the first memory window.


### -field PCD_MemoryCardBase2

<i>Optional</i>, card base address of the second memory window.


### -field PCD_MemoryCardBase

This member is currently unused.


### -field PCD_MemoryFlags

This member is currently unused.


### -field PCD_IoFlags

This member is currently unused.


## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff549665">PCCARD_RESOURCE</a>
 

 
