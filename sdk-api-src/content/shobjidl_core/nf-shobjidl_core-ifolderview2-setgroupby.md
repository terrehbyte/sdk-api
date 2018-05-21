---
UID: NF:shobjidl_core.IFolderView2.SetGroupBy
title: IFolderView2::SetGroupBy
author: windows-driver-content
description: Groups the view by the given property key and direction.
old-location: shell\IFolderView2_SetGroupBy.htm
old-project: shell
ms.assetid: 2d0761cb-7c81-48f7-994d-6dd61062d848
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IFolderView2 interface [Windows Shell],SetGroupBy method, IFolderView2.SetGroupBy, IFolderView2::SetGroupBy, SetGroupBy, SetGroupBy method [Windows Shell], SetGroupBy method [Windows Shell],IFolderView2 interface, _shell_IFolderView2_SetGroupBy, shell.IFolderView2_SetGroupBy, shobjidl_core/IFolderView2::SetGroupBy
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
-	IFolderView2.SetGroupBy
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IFolderView2::SetGroupBy


## -description


Groups the view by the given property key and direction.


## -parameters




### -param key [in]

Type: <b>REFPROPERTYKEY</b>

A <a href="https://msdn.microsoft.com/3f5f31af-f040-443b-9045-9761055381ea">PROPERTYKEY</a> by which the view should be grouped.


### -param fAscending [in]

Type: <b>BOOL</b>

A value of type <b>BOOL</b> to indicate sort order of the groups.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


