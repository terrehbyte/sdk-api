---
UID: NF:shobjidl_core.IObjectProvider.QueryObject
title: IObjectProvider::QueryObject
author: windows-driver-content
description: Queries for a specified object.
old-location: shell\IObjectProvider_QueryObject.htm
old-project: shell
ms.assetid: 7bd76e54-bc1d-481d-90cb-fcfe519b8bfb
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IObjectProvider interface [Windows Shell],QueryObject method, IObjectProvider.QueryObject, IObjectProvider::QueryObject, QueryObject, QueryObject method [Windows Shell], QueryObject method [Windows Shell],IObjectProvider interface, _shell_IObjectProvider_QueryObject, shell.IObjectProvider_QueryObject, shobjidl_core/IObjectProvider::QueryObject
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
-	IObjectProvider.QueryObject
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IObjectProvider::QueryObject


## -description


Queries for a specified object.


## -parameters




### -param guidObject [in]

Type: <b>REFGUID</b>

A reference to the <b>GUID</b> used to identify the object.


### -param riid [in]

Type: <b>REFIID</b>

Specifies the desired interface ID.


### -param ppvOut [out]

Type: <b>void**</b>

On success, contains the address of a pointer to the object specified by <i>riid</i>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Object implementers that want to enable the discovery of other objects that they can produce or that they hold should implement <b>IObjectProvider::QueryObject</b> and publish the <b>GUID</b> values that name those objects for clients of that object. Note that objects should not pass on the request for an object to other objects like <a href="_inet_IServiceProvider_QueryService_Method">QueryService</a>.


