---
UID: NF:mfidl.IMFWorkQueueServicesEx.GetPlatformWorkQueueMMCSSPriority
title: IMFWorkQueueServicesEx::GetPlatformWorkQueueMMCSSPriority
author: windows-sdk-content
description: Gets the priority of the Multimedia Class Scheduler Service (MMCSS) priority associated with the specified platform work queue.
old-location: mf\imfworkqueueservicesex_getplatformworkqueuemmcsspriority.htm
old-project: medfound
ms.assetid: e9271439-8785-4743-9e6f-81342af117f8
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: GetPlatformWorkQueueMMCSSPriority, GetPlatformWorkQueueMMCSSPriority method [Media Foundation], GetPlatformWorkQueueMMCSSPriority method [Media Foundation],IMFWorkQueueServicesEx interface, IMFWorkQueueServicesEx interface [Media Foundation],GetPlatformWorkQueueMMCSSPriority method, IMFWorkQueueServicesEx.GetPlatformWorkQueueMMCSSPriority, IMFWorkQueueServicesEx::GetPlatformWorkQueueMMCSSPriority, mf.imfworkqueueservicesex_getplatformworkqueuemmcsspriority, mfidl/IMFWorkQueueServicesEx::GetPlatformWorkQueueMMCSSPriority
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: MFSensorDeviceMode
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	mfidl.h
api_name:
-	IMFWorkQueueServicesEx.GetPlatformWorkQueueMMCSSPriority
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IMFWorkQueueServicesEx::GetPlatformWorkQueueMMCSSPriority


## -description


Gets the priority of the Multimedia Class Scheduler Service (MMCSS)  priority associated with
    the specified platform work queue.


## -parameters




### -param dwPlatformWorkQueueId [in]

Topology work queue id for which the info will be returned.


### -param plPriority [out]


## -returns



Pointer to a buffer allocated by the caller
    that the work queue's MMCSS task id will be copied to.




## -see-also




<a href="https://msdn.microsoft.com/12d4f0f4-9a6d-4782-b5ae-4add6608782a">IMFWorkQueueServicesEx</a>
 

 
