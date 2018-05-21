---
UID: NF:setupapi.SetupDiSetSelectedDevice
title: SetupDiSetSelectedDevice function
author: windows-driver-content
description: The SetupDiSetSelectedDevice function sets a device information element as the selected member of a device information set. This function is typically used by an installation wizard.
old-location: devinst\setupdisetselecteddevice.htm
old-project: devinst
ms.assetid: d3ce8a05-d26b-452f-8418-e104ae486a1a
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiSetSelectedDevice, SetupDiSetSelectedDevice function [Device and Driver Installation], devinst.setupdisetselecteddevice, di-rtns_db49eaf1-c6cb-48ef-ae17-f5c578672eca.xml, setupapi/SetupDiSetSelectedDevice
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Setupapi.dll
api_name:
-	SetupDiSetSelectedDevice
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiSetSelectedDevice function


## -description


The <b>SetupDiSetSelectedDevice</b> function sets a device information element as the selected member of a device information set. This function is typically used by an installation wizard.


## -parameters




### -param DeviceInfoSet [in]

A handle to the <a href="devinst.device_information_sets">device information set</a> that contains the device information element to set as the selected member of the device information set. 


### -param DeviceInfoData [in]

A pointer to an <a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a> structure that specifies the device information element in <i>DeviceInfoSet</i> to set as the selected member of <i>DeviceInfoSet</i>.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved with a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff552011">SetupDiGetSelectedDevice</a>
 

 
