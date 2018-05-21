---
UID: NF:shobjidl_core.IApplicationDesignModeSettings2.GetApplicationViewOrientation
title: IApplicationDesignModeSettings2::GetApplicationViewOrientation
author: windows-driver-content
description: Gets the orientation of the application design mode window.
old-location: shell\IApplicationDesignModeSettings2_GetApplicationViewOrientation.htm
old-project: shell
ms.assetid: D6DF8432-7D37-4D39-9E08-2F5B874A0BCB
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetApplicationViewOrientation, GetApplicationViewOrientation method [Windows Shell], GetApplicationViewOrientation method [Windows Shell],IApplicationDesignModeSettings2 interface, IApplicationDesignModeSettings2 interface [Windows Shell],GetApplicationViewOrientation method, IApplicationDesignModeSettings2.GetApplicationViewOrientation, IApplicationDesignModeSettings2::GetApplicationViewOrientation, shell.IApplicationDesignModeSettings2_GetApplicationViewOrientation, shobjidl_core/IApplicationDesignModeSettings2::GetApplicationViewOrientation
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
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
-	twinapi.dll
api_name:
-	IApplicationDesignModeSettings2.GetApplicationViewOrientation
product: Windows
targetos: Windows
req.lib: Twinapi.lib
req.dll: Twinapi.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IApplicationDesignModeSettings2::GetApplicationViewOrientation


## -description


Gets the orientation of the application design mode window.


## -parameters




### -param applicationSizePixels




### -param viewOrientation [out]

Type: <b><a href="https://msdn.microsoft.com/6E14D892-09E3-46F4-84AD-991996431FB2">APPLICATION_VIEW_ORIENTATION</a>*</b>

When this method returns successfully, receives a pointer to an  <a href="https://msdn.microsoft.com/6E14D892-09E3-46F4-84AD-991996431FB2">APPLICATION_VIEW_ORIENTATION</a> structure.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/1F630AFF-3C73-461C-AE41-D597F6FF42D8">IApplicationDesignModeSettings2</a>
 

 
