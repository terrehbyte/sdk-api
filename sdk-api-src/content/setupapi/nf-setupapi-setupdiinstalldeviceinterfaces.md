---
UID: NF:setupapi.SetupDiInstallDeviceInterfaces
title: SetupDiInstallDeviceInterfaces function
author: windows-driver-content
description: The SetupDiInstallDeviceInterfaces function is the default handler for the DIF_INSTALLINTERFACES installation request.
old-location: devinst\setupdiinstalldeviceinterfaces.htm
old-project: devinst
ms.assetid: c47d83f6-9ae5-43a9-a6ed-b0441b490e8d
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiInstallDeviceInterfaces, SetupDiInstallDeviceInterfaces function [Device and Driver Installation], devinst.setupdiinstalldeviceinterfaces, di-rtns_8bb9c70f-c1be-45f6-af6c-243a750babb9.xml, setupapi/SetupDiInstallDeviceInterfaces
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
-	SetupDiInstallDeviceInterfaces
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiInstallDeviceInterfaces function


## -description


The <b>SetupDiInstallDeviceInterfaces</b> function is the default handler for the <a href="https://msdn.microsoft.com/library/windows/hardware/ff543695">DIF_INSTALLINTERFACES</a> installation request. 


## -parameters




### -param DeviceInfoSet [in]

A pointer to the <a href="devinst.device_information_sets">device information set</a> that contains a device information element that represents the device for which to install interfaces. The device information set must contain only elements for the local system.


### -param DeviceInfoData [in]

A pointer to an <a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a> structure that specifies the device information element in <i>DeviceInfoSet</i>.


## -returns



<b>SetupDiInstallDeviceInterfaces</b> returns <b>TRUE</b> if the function completed without error. If the function completed with an error, <b>FALSE</b> is returned and the error code for the failure can be retrieved by calling <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



<b>SetupDiInstallDeviceInterfaces</b> processes each <b>AddInterface</b> entry in the <i>DDInstall</i>.<b>Interfaces</b> section of a device INF file and creates each interface by calling <a href="https://msdn.microsoft.com/library/windows/hardware/ff550965">SetupDiCreateDeviceInterface</a>.

The caller of <b>SetupDiInstallDeviceInterfaces</b> must be a member of the Administrators group. 

<div class="alert"><b>Note</b>  Only a <a href="https://msdn.microsoft.com/ac439eb8-b491-4215-877d-5ee177fbdb39">class installer</a> should call <b>SetupDiInstallDeviceInterfaces</b> and only in those situations where the class installer must perform device interface installation operations after <b>SetupDiInstallDeviceInterfaces</b> completes the default device interface installation operation. In such situations, the class installer must directly call <b>SetupDiInstallDeviceInterfaces</b>when the installer processes a DIF_INSTALLINTERFACES request. For more information about calling the default handler, see <a href="devinst.calling_the_default_dif_code_handlers">Calling Default DIF Code Handlers</a>.</div>
<div> </div>
For information about INF file format, see <a href="devinst.inf_file_sections_and_directives">INF File Sections and Directives</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff543695">DIF_INSTALLINTERFACES</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550965">SetupDiCreateDeviceInterface</a>
 

 
