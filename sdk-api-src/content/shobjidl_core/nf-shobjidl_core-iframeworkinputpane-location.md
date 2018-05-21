---
UID: NF:shobjidl_core.IFrameworkInputPane.Location
title: IFrameworkInputPane::Location
author: windows-driver-content
description: Gets the current location of the input pane.
old-location: shell\IFrameworkInputPane_Location.htm
old-project: shell
ms.assetid: 2633AD19-318E-419f-9B40-16E65803285E
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IFrameworkInputPane interface [Windows Shell],Location method, IFrameworkInputPane.Location, IFrameworkInputPane::Location, Location, Location method [Windows Shell], Location method [Windows Shell],IFrameworkInputPane interface, shell.IFrameworkInputPane_Location, shobjidl_core/IFrameworkInputPane::Location
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
-	IFrameworkInputPane.Location
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFrameworkInputPane::Location


## -description


Gets the current location of the input pane.


## -parameters




### -param prcInputPaneScreenLocation [out]

Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a> structure that, when this method returns successfully, receives the location of the input pane, in screen coordinates. If the input pane is not visible, this structure receives an empty rectangle.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/05C115BA-249A-4271-9C6F-DAAEE91BB936">IFrameworkInputPane</a>
 

 
