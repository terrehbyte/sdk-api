---
UID: NF:shobjidl_core.IExplorerBrowser.SetRect
title: IExplorerBrowser::SetRect
author: windows-driver-content
description: Sets the size and position of the view windows created by the browser.
old-location: shell\IExplorerBrowser_SetRect.htm
old-project: shell
ms.assetid: 392052ea-1053-4f55-96aa-2d64b0ee0390
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IExplorerBrowser interface [Windows Shell],SetRect method, IExplorerBrowser.SetRect, IExplorerBrowser::SetRect, SetRect, SetRect method [Windows Shell], SetRect method [Windows Shell],IExplorerBrowser interface, _shell_IExplorerBrowser_SetRect, shell.IExplorerBrowser_SetRect, shobjidl_core/IExplorerBrowser::SetRect
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
-	IExplorerBrowser.SetRect
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IExplorerBrowser::SetRect


## -description


Sets the size and position of the view windows created by the browser.


## -parameters




### -param phdwp [in, out]

Type: <b>HDWP*</b>

A pointer to a <a href="https://msdn.microsoft.com/2758de7b-c218-4a9b-b11b-b189301f7514">DeferWindowPos</a> handle. This parameter can be <b>NULL</b>.


### -param rcBrowser [in]

Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">RECT</a></b>

The coordinates that the browser will occupy.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Coordinates are relative to the <i>hwndParent</i> passed in <a href="https://msdn.microsoft.com/4b86646a-a20c-4bb5-a4c8-5c2e11e18862">IExplorerBrowser::Initialize</a>.


