---
UID: NF:shobjidl_core.SHAssocEnumHandlers
title: SHAssocEnumHandlers function
author: windows-driver-content
description: Returns an enumeration object for a specified set of file name extension handlers.
old-location: shell\SHAssocEnumHandlers.htm
old-project: shell
ms.assetid: 83db466b-e00c-4015-879f-c5c222f45b8c
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ASSOC_FILTER_NONE, ASSOC_FILTER_RECOMMENDED, SHAssocEnumHandlers, SHAssocEnumHandlers function [Windows Shell], _shell_SHAssocEnumHandlers, shell.SHAssocEnumHandlers, shobjidl_core/SHAssocEnumHandlers
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Shell32.dll
api_name:
-	SHAssocEnumHandlers
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# SHAssocEnumHandlers function


## -description


Returns an enumeration object for a specified set of file name extension handlers.


## -parameters




### -param pszExtra [in]

Type: <b>PCWSTR</b>

A pointer to a null-terminated buffer that contains a single file type extension, for instance ".jpg". Only handlers associated with the given extension are enumerated. If this value is <b>NULL</b>, all handlers for all extensions are enumerated.


### -param afFilter [in]

Type: <b>ASSOC_FILTER</b>

Specifies the enumeration handler filter applied to the full list of handlers that results from the value given in <i>pszExtra</i>. One of the following values.



#### ASSOC_FILTER_NONE

Return all handlers.



#### ASSOC_FILTER_RECOMMENDED

Return only recommended handlers. A handler sets its recommended status in the registry when it is installed. An initial status of non-recommended can later be promoted to recommended as a result of user action.


### -param ppEnumHandler [out]

Type: <b><a href="https://msdn.microsoft.com/c8b11157-4d00-4ab1-aea5-ce8ae35c43ce">IEnumAssocHandlers</a>**</b>

When this method returns, contains the address of a pointer to an <a href="https://msdn.microsoft.com/c8b11157-4d00-4ab1-aea5-ce8ae35c43ce">IEnumAssocHandlers</a> object.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


