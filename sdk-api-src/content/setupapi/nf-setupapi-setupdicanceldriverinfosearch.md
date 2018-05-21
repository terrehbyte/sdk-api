---
UID: NF:setupapi.SetupDiCancelDriverInfoSearch
title: SetupDiCancelDriverInfoSearch function
author: windows-driver-content
description: The SetupDiCancelDriverInfoSearch function cancels a driver list search that is currently in progress in a different thread.
old-location: devinst\setupdicanceldriverinfosearch.htm
old-project: devinst
ms.assetid: 847f1f5e-5634-44ea-b530-6136629f0471
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiCancelDriverInfoSearch, SetupDiCancelDriverInfoSearch function [Device and Driver Installation], devinst.setupdicanceldriverinfosearch, di-rtns_6cdb6cd3-5d8d-4af6-b747-b585d9c25df4.xml, setupapi/SetupDiCancelDriverInfoSearch
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
-	SetupDiCancelDriverInfoSearch
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiCancelDriverInfoSearch function


## -description


The <b>SetupDiCancelDriverInfoSearch</b> function cancels a driver list search that is currently in progress in a different thread. 


## -parameters




### -param DeviceInfoSet [in]

A handle to the <a href="devinst.device_information_sets">device information set</a> for which a driver list is being built.


## -returns



If a driver list search is underway for the specified device information set when this function is called, the search is terminated. <b>SetupDiCancelDriverInfoSearch</b> returns <b>TRUE</b> when the termination is confirmed. Otherwise, it returns <b>FALSE</b> and a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> returns ERROR_INVALID_HANDLE. 




## -remarks



<b>SetupDiCancelDriverInfoSearch</b> is a synchronous call. Therefore, it does not return until the driver search thread responds to the termination request.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550917">SetupDiBuildDriverInfoList</a>
 

 
