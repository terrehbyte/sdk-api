---
UID: NF:shobjidl_core.IShellItem2.GetProperty
title: IShellItem2::GetProperty
author: windows-driver-content
description: Gets a PROPVARIANT structure from a specified property key.
old-location: shell\IShellItem2_GetProperty.htm
old-project: shell
ms.assetid: f72e23b9-e99b-462b-91b6-9ef27a4fc9e1
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetProperty, GetProperty method [Windows Shell], GetProperty method [Windows Shell],IShellItem2 interface, IShellItem2 interface [Windows Shell],GetProperty method, IShellItem2.GetProperty, IShellItem2::GetProperty, _shell_IShellItem2_GetProperty, shell.IShellItem2_GetProperty, shobjidl_core/IShellItem2::GetProperty
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
-	IShellItem2.GetProperty
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IShellItem2::GetProperty


## -description


Gets a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure from a specified property key.


## -parameters




### -param key [in]

Type: <b>REFPROPERTYKEY</b>

A reference to a <a href="https://msdn.microsoft.com/3f5f31af-f040-443b-9045-9761055381ea">PROPERTYKEY</a> structure.


### -param ppropvar [out]

Type: <b><a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a>*</b>

Contains a pointer to a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> structure.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


