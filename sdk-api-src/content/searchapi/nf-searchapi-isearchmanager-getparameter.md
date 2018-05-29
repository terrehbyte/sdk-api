---
UID: NF:searchapi.ISearchManager.GetParameter
title: ISearchManager::GetParameter
author: windows-sdk-content
description: Not supported.This method returns E_INVALIDARG when called.
old-location: search\_search_ISearchManager_GetParameter.htm
old-project: search
ms.assetid: VS|search|~\search\wds3x\reference\ifaces\indexmanagement\isearchmanager\getparameter.htm
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: GetParameter, GetParameter method [search], GetParameter method [search],ISearchManager interface, ISearchManager interface [search],GetParameter method, ISearchManager.GetParameter, ISearchManager::GetParameter, _search_ISearchManager_GetParameter, search._search_ISearchManager_GetParameter, searchapi/ISearchManager::GetParameter
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: searchapi.h
req.include-header: Searchapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 with SP1 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Searchadmin.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: ROWSETEVENT_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	searchapi.h
api_name:
-	ISearchManager.GetParameter
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ISearchManager::GetParameter


## -description


Not supported.

This method returns E_INVALIDARG when called.


## -parameters




### -param pszName [in]

Type: <b>LPCWSTR</b>


                    There are currently no valid parameters in this version of search (WDS 3.0).


### -param ppValue [out, retval]

Type: <b><a href="_stg_propvariant">PROPVARIANT</a>**</b>


                    Returns a value in an undefined state as there are no properties currently defined to retrieve values from.


## -returns



Type: <b>HRESULT</b>

This method returns E_InvalidArg as an error code when called.




## -remarks



The ReindexMatchingUrls code sample, available on <a href="http://go.microsoft.com/fwlink/p/?linkid=155654">Code Gallery</a> and the <a href="http://go.microsoft.com/fwlink/p/?linkid=129787">Windows 7 SDK</a>, demonstrates ways to specify which files to re-index and how.


