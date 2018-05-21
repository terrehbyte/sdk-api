---
UID: NS:cfgmgr32.DMA_Range_s
title: DMA_Range_s
author: windows-driver-content
description: The DMA_RANGE structure specifies a resource requirements list that describes DMA channel usage for a device instance. For more information about resource requirements lists, see Hardware Resources.
old-location: devinst\dma_range.htm
old-project: devinst
ms.assetid: 46c80013-1863-4e02-be8d-282d2e619200
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: "*PDMA_RANGE, DMA_RANGE, DMA_RANGE structure [Device and Driver Installation], DMA_Range_s, PDMA_RANGE, PDMA_RANGE structure pointer [Device and Driver Installation], cfgmgr32/DMA_RANGE, cfgmgr32/PDMA_RANGE, cfgmgrst_a19d993e-d664-4218-8bae-23e97919b3a8.xml, devinst.dma_range"
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
req.typenames: DMA_RANGE, *PDMA_RANGE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	cfgmgr32.h
api_name:
-	DMA_RANGE
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# DMA_Range_s structure


## -description


The DMA_RANGE structure specifies a resource requirements list that describes DMA channel usage for a device instance. For more information about resource requirements lists, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff547012">Hardware Resources</a>.


## -struct-fields




### -field DR_Min

The lowest-numbered DMA channel that can be allocated to the device.


### -field DR_Max

The highest-numbered DMA channel that can be allocated to the device.


### -field DR_Flags

One bit flag from <i>each</i> of the flag sets described in the table included with the description of the <b>DR_Flags</b> member of the <a href="https://msdn.microsoft.com/library/windows/hardware/ff544758">DMA_DES</a> structure.


## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff544758">DMA_DES</a>
 

 
