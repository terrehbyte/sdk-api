---
UID: NF:shobjidl_core.IApplicationDesignModeSettings.SetApplicationViewState
title: IApplicationDesignModeSettings::SetApplicationViewState
author: windows-driver-content
description: Sets a spoofed application view state (full-screen landscape, full-screen portrait, filled, or snapped) to be used for a Windows Store app running in design mode.
old-location: shell\IApplicationDesignModeSettings_SetApplicationViewState.htm
old-project: shell
ms.assetid: 37e1845c-a58a-4da3-b259-bbf5bbf5ff6d
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IApplicationDesignModeSettings interface [Windows Shell],SetApplicationViewState method, IApplicationDesignModeSettings.SetApplicationViewState, IApplicationDesignModeSettings::SetApplicationViewState, SetApplicationViewState, SetApplicationViewState method [Windows Shell], SetApplicationViewState method [Windows Shell],IApplicationDesignModeSettings interface, shell.IApplicationDesignModeSettings_SetApplicationViewState, shobjidl_core/IApplicationDesignModeSettings::SetApplicationViewState
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
-	Twinapi.dll
api_name:
-	IApplicationDesignModeSettings.SetApplicationViewState
product: Windows
targetos: Windows
req.lib: 
req.dll: Twinapi.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IApplicationDesignModeSettings::SetApplicationViewState


## -description


Sets a spoofed application view state (full-screen landscape, full-screen portrait, filled, or snapped) to be used for a Windows Store app running in design mode.

You must call <a href="https://msdn.microsoft.com/429E5D12-9ED9-4f4f-A0E6-F95953C9113A">IInitializeWithWindow::Initialize</a> to set a proxy core window before calling this method.

<b>SetApplicationViewState</b> must be called before calling <a href="https://msdn.microsoft.com/1ac42bb8-1c24-4369-8d0d-db3ad4062501">ComputeApplicationSize</a>.


## -parameters




### -param viewState [in]

One of the <a href="https://msdn.microsoft.com/A79F66BD-2972-4f30-9284-E88B8201F38D">APPLICATION_VIEW_STATE</a> enumeration values that indicates the application view state to spoof.


## -returns



If this method succeeds, it returns S_OK. Otherwise, it returns an HRESULT error code, including the following:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOT_SET</b></dt>
</dl>
</td>
<td width="60%">

<a href="https://msdn.microsoft.com/429E5D12-9ED9-4f4f-A0E6-F95953C9113A">IInitializeWithWindow::Initialize</a> has not been called to set a proxy core window.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/D26C9A87-8C29-4029-BF8A-E0566DC2DF2A">IApplicationDesignModeSettings</a>
 

 
