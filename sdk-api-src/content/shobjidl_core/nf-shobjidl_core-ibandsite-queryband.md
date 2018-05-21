---
UID: NF:shobjidl_core.IBandSite.QueryBand
title: IBandSite::QueryBand
author: windows-driver-content
description: Gets information about a band in a band site.
old-location: shell\IBandSite_QueryBand.htm
old-project: shell
ms.assetid: 0618ad7d-4e8f-4fbf-ab64-2b1c0d42158c
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IBandSite interface [Windows Shell],QueryBand method, IBandSite.QueryBand, IBandSite::QueryBand, QueryBand, QueryBand method [Windows Shell], QueryBand method [Windows Shell],IBandSite interface, _win32_IBandSite_QueryBand, shell.IBandSite_QueryBand, shobjidl_core/IBandSite::QueryBand
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shldisp.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shldisp.idl
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
-	IBandSite.QueryBand
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.71 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IBandSite::QueryBand


## -description


Gets information about a band in a band site.


## -parameters




### -param dwBandID [in]

Type: <b>DWORD</b>

The ID of the band object to query.


### -param ppstb [out, optional]

Type: <b><a href="https://msdn.microsoft.com/eb9f7f2a-a6be-4527-8a32-325dad4c8000">IDeskBand</a>**</b>

Address of an <a href="https://msdn.microsoft.com/eb9f7f2a-a6be-4527-8a32-325dad4c8000">IDeskBand</a> interface pointer that, when this method returns successfully, points to the <b>IDeskBand</b> object that represents the band. This value can be <b>NULL</b>.


### -param pdwState [out, optional]

Type: <b>DWORD*</b>

Pointer to a <b>DWORD</b> value that, when this method returns successfully, receives the state of the band object. This state is a combination of BSSF_VISIBLE, BSSF_NOTITLE, and BSSF_UNDELETEABLE. See <a href="https://msdn.microsoft.com/86e4afce-594a-441e-b6d9-ce05c8234150">BANDSITEINFO</a> for more information on those flags. This value can be <b>NULL</b> if the state information is not needed.


### -param pszName [out]

Type: <b>LPWSTR</b>

Pointer to a buffer of <i>cchName</i> Unicode characters that, when this method returns successfully, receives the name of the band object.


### -param cchName [in]

Type: <b>int</b>

The size of the <i>pszName</i> buffer, in characters.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


