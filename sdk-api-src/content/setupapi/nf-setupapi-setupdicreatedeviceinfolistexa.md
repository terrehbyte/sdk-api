---
UID: NF:setupapi.SetupDiCreateDeviceInfoListExA
title: SetupDiCreateDeviceInfoListExA function
author: windows-sdk-content
description: The SetupDiCreateDeviceInfoList function creates an empty device information set on a remote or a local computer and optionally associates the set with a device setup class .
old-location: devinst\setupdicreatedeviceinfolistex.htm
old-project: devinst
ms.assetid: 4dae7b07-2e24-4fd8-82f2-f947296ce3c4
ms.author: windowssdkdev
ms.date: 05/31/2018
ms.keywords: SetupDiCreateDeviceInfoListEx, SetupDiCreateDeviceInfoListEx function [Device and Driver Installation], SetupDiCreateDeviceInfoListExA, SetupDiCreateDeviceInfoListExW, devinst.setupdicreatedeviceinfolistex, di-rtns_584dc470-c07f-4658-b16d-53a2594dabf9.xml, setupapi/SetupDiCreateDeviceInfoListEx
ms.prod: windows
ms.technology: windows-sdk
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
tech.root: 
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Setupapi.lib
 - Setupapi.dll
api_name:
 - SetupDiCreateDeviceInfoListEx
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# SetupDiCreateDeviceInfoListExA function


## -description


The <b>SetupDiCreateDeviceInfoList</b> function creates an empty <a href="devinst.device_information_sets">device information set</a> on a remote or a local computer and optionally associates the set with a device setup class .


## -parameters




### -param ClassGuid [in, optional]

A pointer to the GUID of the device setup class to associate with the newly created device information set. If this parameter is specified, only devices of this class can be included in this device information set. If this parameter is set to <b>NULL</b>, the device information set is not associated with a specific device setup class.


### -param hwndParent [in, optional]

A handle to the top-level window to use for any user interface that is related to non-device-specific actions (such as a select-device dialog box that uses the global class driver list). This handle is optional and can be <b>NULL</b>. If a specific top-level window is not required, set <i>hwndParent</i> to <b>NULL</b>.


### -param MachineName [in, optional]

A pointer to a NULL-terminated string that contains the name of a computer on a network. If a name is specified, only devices on that computer can be created and opened in this device information set. If this parameter is set to <b>NULL</b>, the device information set is for devices on the local computer.


### -param Reserved

Must be <b>NULL</b>.


## -returns



The function returns a handle to an empty device information set if it is successful. Otherwise, it returns INVALID_HANDLE_VALUE. To get extended error information, call <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



The caller of this function must delete the returned device information set when it is no longer needed by calling <a href="https://msdn.microsoft.com/library/windows/hardware/ff550996">SetupDiDestroyDeviceInfoList</a>. 

If the device information set is for devices on a remote computer (<i>MachineName</i> is not <b>NULL</b>), all subsequent operations on this set or any of its elements must use routines that support device information sets with remote elements. The <b>SetupDi</b><i>Xxx</i> routines that do not provide this support, such as <a href="https://msdn.microsoft.com/library/windows/hardware/ff550922">SetupDiCallClassInstaller</a>, have a statement to that effect in their reference page.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550956">SetupDiCreateDeviceInfoList</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550996">SetupDiDestroyDeviceInfoList</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551103">SetupDiGetDeviceInfoListDetail</a>
 

 
