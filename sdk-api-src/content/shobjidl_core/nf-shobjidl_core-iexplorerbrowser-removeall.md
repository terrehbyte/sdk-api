---
UID: NF:shobjidl_core.IExplorerBrowser.RemoveAll
title: IExplorerBrowser::RemoveAll
author: windows-driver-content
description: Removes all items from the results folder.
old-location: shell\IExplorerBrowser_RemoveAll.htm
old-project: shell
ms.assetid: 4447d3f4-659f-4ec1-8a6f-91031c85b704
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IExplorerBrowser interface [Windows Shell],RemoveAll method, IExplorerBrowser.RemoveAll, IExplorerBrowser::RemoveAll, RemoveAll, RemoveAll method [Windows Shell], RemoveAll method [Windows Shell],IExplorerBrowser interface, _shell_IExplorerBrowser_RemoveAll, shell.IExplorerBrowser_RemoveAll, shobjidl_core/IExplorerBrowser::RemoveAll
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
-	IExplorerBrowser.RemoveAll
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IExplorerBrowser::RemoveAll


## -description


Removes all items from the results folder.


## -parameters






## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or  E_UNEXPECTED if this method is called before a call to <a href="https://msdn.microsoft.com/f978d5d1-a597-4e49-9a2a-de23e99bf65e">IExplorerBrowser::FillFromObject</a>.




## -remarks



This method removes all results from the  <a href="https://msdn.microsoft.com/db44052b-bd26-412f-9f2a-66a0c53b65ac">IResultsFolder</a> created in method <a href="https://msdn.microsoft.com/f978d5d1-a597-4e49-9a2a-de23e99bf65e">IExplorerBrowser::FillFromObject</a>.


