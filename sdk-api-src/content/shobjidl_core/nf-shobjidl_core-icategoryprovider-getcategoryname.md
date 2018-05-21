---
UID: NF:shobjidl_core.ICategoryProvider.GetCategoryName
title: ICategoryProvider::GetCategoryName
author: windows-driver-content
description: Gets the name of the specified category.
old-location: shell\ICategoryProvider_GetCategoryName.htm
old-project: shell
ms.assetid: 3730394a-8720-46cc-a9da-cd5cf0df7eeb
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetCategoryName, GetCategoryName method [Windows Shell], GetCategoryName method [Windows Shell],ICategoryProvider interface, ICategoryProvider interface [Windows Shell],GetCategoryName method, ICategoryProvider.GetCategoryName, ICategoryProvider::GetCategoryName, inet_ICategoryProvider_GetCategoryName, shell.ICategoryProvider_GetCategoryName, shobjidl_core/ICategoryProvider::GetCategoryName
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
-	ICategoryProvider.GetCategoryName
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# ICategoryProvider::GetCategoryName


## -description


Gets the name of the specified category.


## -parameters




### -param pguid [in]

Type: <b>const GUID*</b>

A pointer to a GUID.


### -param pszName [out]

Type: <b>LPWSTR</b>

When this method returns, contains a pointer to a string that receives the name of the category.


### -param cch [in]

Type: <b>UINT</b>

An integer that receives the number of characters in the string.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


