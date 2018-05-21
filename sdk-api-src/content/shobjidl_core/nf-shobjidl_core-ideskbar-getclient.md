---
UID: NF:shobjidl_core.IDeskBar.GetClient
title: IDeskBar::GetClient
author: windows-driver-content
description: Gets the client object.
old-location: shell\IDeskBar_GetClient.htm
old-project: shell
ms.assetid: 003b400c-03a4-47c0-a6b8-04aa65ac573c
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetClient, GetClient method [Windows Shell], GetClient method [Windows Shell],IDeskBar interface, IDeskBar interface [Windows Shell],GetClient method, IDeskBar.GetClient, IDeskBar::GetClient, _win32_IDeskBar_GetClient, shell.IDeskBar_GetClient, shobjidl_core/IDeskBar::GetClient
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
-	Shell32.dll
api_name:
-	IDeskBar.GetClient
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IDeskBar::GetClient


## -description


Gets the client object.


## -parameters




### -param ppunkClient [out]

Type: <b><a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>**</b>


          The address of a pointer to a variable of type <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> that receives the client used by the desk bar.
        


## -returns



Type: <b>HRESULT</b>

Returns S_OK if the client object is returned, or an error value otherwise.


