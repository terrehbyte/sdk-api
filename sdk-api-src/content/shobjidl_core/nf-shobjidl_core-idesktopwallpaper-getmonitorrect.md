---
UID: NF:shobjidl_core.IDesktopWallpaper.GetMonitorRECT
title: IDesktopWallpaper::GetMonitorRECT
author: windows-driver-content
description: Retrieves the display rectangle of the specified monitor.
old-location: shell\IDesktopWallpaper_GetMonitorRECT.htm
old-project: shell
ms.assetid: 98A3F193-DBCF-42ec-9283-53F0F46BB1C4
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetMonitorRECT, GetMonitorRECT method [Windows Shell], GetMonitorRECT method [Windows Shell],IDesktopWallpaper interface, IDesktopWallpaper interface [Windows Shell],GetMonitorRECT method, IDesktopWallpaper.GetMonitorRECT, IDesktopWallpaper::GetMonitorRECT, shell.IDesktopWallpaper_GetMonitorRECT, shobjidl_core/IDesktopWallpaper::GetMonitorRECT
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	shobjidl_core.h
api_name:
-	IDesktopWallpaper.GetMonitorRECT
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IDesktopWallpaper::GetMonitorRECT


## -description


Retrieves the display rectangle of the specified monitor.


## -parameters




### -param monitorID [in]

The ID of the monitor to query. You can get this value through <a href="https://msdn.microsoft.com/CE0C6B07-F9D1-4221-9D9D-8D17CF6780E6">GetMonitorDevicePathAt</a>.


### -param displayRect [out]

A pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a> structure that, when this method returns successfully, receives the display rectangle of the monitor specified by <i>monitorID</i>, in screen coordinates.


## -returns



If this method succeeds, it returns <b>S_OK</b>. Otherwise, it returns an <b>HRESULT</b> error code, including the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The monitor specified by <i>monitorID</i> is not currently attached to the system.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A <b>NULL</b> pointer was provided in <i>displayRect</i>.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The ID supplied in <i>monitorID</i> cannot be found.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/A83903B5-314B-4a8b-8D37-F8A8995DE0CB">IDesktopWallpaper</a>
 

 
