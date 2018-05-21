---
UID: NF:shobjidl_core.IDragSourceHelper.InitializeFromBitmap
title: IDragSourceHelper::InitializeFromBitmap
author: windows-driver-content
description: Initializes the drag-image manager for a windowless control.
old-location: shell\IDragSourceHelper_InitializeFromBitmap.htm
old-project: shell
ms.assetid: d50be9c9-f407-4386-bb8f-04c849205359
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IDragSourceHelper interface [Windows Shell],InitializeFromBitmap method, IDragSourceHelper.InitializeFromBitmap, IDragSourceHelper::InitializeFromBitmap, InitializeFromBitmap, InitializeFromBitmap method [Windows Shell], InitializeFromBitmap method [Windows Shell],IDragSourceHelper interface, _win32_IDragSourceHelper_InitializeFromBitmap, shell.IDragSourceHelper_InitializeFromBitmap, shobjidl_core/IDragSourceHelper::InitializeFromBitmap
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
-	IDragSourceHelper.InitializeFromBitmap
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IDragSourceHelper::InitializeFromBitmap


## -description


Initializes the drag-image manager for a windowless control.


## -parameters




### -param pshdi [in]

Type: <b>LPSHDRAGIMAGE</b>

The <a href="https://msdn.microsoft.com/e0dd76b2-fd5c-41e8-b540-db90a2f0dcec">SHDRAGIMAGE</a> structure that contains information about the bitmap.


### -param pDataObject [in]

Type: <b><a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a>*</b>

A pointer to the data object's <a href="https://msdn.microsoft.com/8a002deb-2727-456c-8078-a9b0d5893ed4">IDataObject</a> interface.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Because <b>InitializeFromBitmap</b> always performs the RGB multiplication step in calculating the alpha value, you should always pass a bitmap without premultiplied alpha blending. Note that no error will result from passing the method a bitmap with premultiplied alpha blending, but this method will multiply it again, doubling the resulting alpha value.




## -see-also




<a href="https://msdn.microsoft.com/d68ac8fd-4d9c-47ee-bdff-0c5bae6b5e28">IDragSourceHelper</a>
 

 
