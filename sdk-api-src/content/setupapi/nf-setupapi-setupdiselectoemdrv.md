---
UID: NF:setupapi.SetupDiSelectOEMDrv
title: SetupDiSelectOEMDrv function
author: windows-driver-content
description: The SetupDiSelectOEMDrv function selects a driver for a device information set or a particular device information element that uses an OEM path supplied by the user.
old-location: devinst\setupdiselectoemdrv.htm
old-project: devinst
ms.assetid: e97f0569-419a-4a9a-a657-fd972b160269
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiSelectOEMDrv, SetupDiSelectOEMDrv function [Device and Driver Installation], devinst.setupdiselectoemdrv, di-rtns_00ac5dd3-d358-4f14-b8ea-20231051ed8d.xml, setupapi/SetupDiSelectOEMDrv
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
-	SetupDiSelectOEMDrv
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiSelectOEMDrv function


## -description


The <b>SetupDiSelectOEMDrv</b> function selects a driver for a device information set or a particular device information element that uses an OEM path supplied by the user.


## -parameters




### -param hwndParent [in, optional]

A window handle that will be the parent of any dialogs created during the processing of this function. This parameter can be used to override the <b>hwndParent</b> field in the installation parameters block of the specified device information set or element. 


### -param DeviceInfoSet [in]

A handle to the <a href="devinst.device_information_sets">device information set</a> for which to select a driver. 


### -param DeviceInfoData [in, out]

A pointer to an <a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a> structure that specifies a device information element in <i>DeviceInfoSet</i>. This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <b>SetupDiSelectOEMDrv</b> associates the selected driver with the specified device. If this parameter is <b>NULL</b>, <b>SetupDiSelectOEMDrv</b> associates the selected driver with the global class driver list for <i>DeviceInfoSet</i>.  


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved by a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



<b>SetupDiSelectOEMDrv </b>is primarily designed to select an OEM driver for a device on a local computer before installing the device on that computer. Although <b>SetupDiSelectOEMDrv</b> will not fail if the device information set is for a remote computer, the result is of limited use because the device information set cannot subsequently be used with DIF_<i>Xxx</i> installation requests or <b>SetupDi</b><i>Xxx</i> functions that do not support operations on a remote computer. In particular, the device information set cannot be used as input with a DIF_INSTALLDEVICE installation request to install a device on a remote computer.

<b>SetupDiSelectOEMDrv</b> prompts the user for the OEM path and then calls the class installer to select a driver from the OEM path.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550905">SetupDiAskForOEMDisk</a>
 

 
