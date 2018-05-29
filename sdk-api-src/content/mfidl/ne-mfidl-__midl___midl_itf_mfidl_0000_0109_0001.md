---
UID: NE:mfidl.__MIDL___MIDL_itf_mfidl_0000_0109_0001
title: "__MIDL___MIDL_itf_mfidl_0000_0109_0001"
author: windows-sdk-content
description: Specifies the type of a sensor device. A value from this enumeration is returned by IMFSensorDevice::GetDeviceType.
old-location: mf\mfsensordevicetype.htm
old-project: medfound
ms.assetid: 13CC03E6-F0E2-4E69-B94F-4CF1BC7D0C23
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: MFSensorDeviceType, MFSensorDeviceType enumeration [Media Foundation], MFSensorDeviceType_Device, MFSensorDeviceType_FrameProvider, MFSensorDeviceType_MediaSource, MFSensorDeviceType_Unknown, __MIDL___MIDL_itf_mfidl_0000_0109_0001, mf.mfsensordevicetype, mfidl/MFSensorDeviceType, mfidl/MFSensorDeviceType_Device, mfidl/MFSensorDeviceType_FrameProvider, mfidl/MFSensorDeviceType_MediaSource, mfidl/MFSensorDeviceType_Unknown
ms.prod: windows
ms.technology: windows-sdk
ms.topic: enum
req.header: mfidl.h
req.include-header: 
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
req.typenames: MFSensorDeviceType
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	mfidl.h
api_name:
-	MFSensorDeviceType
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# __MIDL___MIDL_itf_mfidl_0000_0109_0001 enumeration


## -description


Specifies the type of a sensor device. A value from this enumeration is returned by <a href="https://msdn.microsoft.com/6714B5A8-83F2-44CD-B061-749EA6BFBF20">IMFSensorDevice::GetDeviceType</a>.


## -enum-fields




### -field MFSensorDeviceType_Unknown

The sensor device type is unknown.


### -field MFSensorDeviceType_Device

The sensor device is a physical device. Physical cameras may register as <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff548567(v=vs.85).aspx">KSCATEGORY_SENSOR_CAMERA</a> or <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff548567(v=vs.85).aspx">KSCATEGORY_VIDEO_CAMERA</a>  or both.


### -field MFSensorDeviceType_MediaSource

The sensor device is a custom media source.


### -field MFSensorDeviceType_FrameProvider

The sensor device is a legacy frame provider.


### -field MFSensorDeviceType_SensorTransform


