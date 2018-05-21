---
UID: NF:tapi3if.ITPhone.put_RingMode
title: ITPhone::put_RingMode
author: windows-driver-content
description: The put_RingMode method requests that the phone change its ring mode.
old-location: tapi3\itphone_put_ringmode.htm
old-project: Tapi
ms.assetid: f693bf24-540d-4509-bf0c-01be27f823f8
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITPhone interface [TAPI 2.2],put_RingMode method, ITPhone.put_RingMode, ITPhone::put_RingMode, _tapi3_itphone_put_ringmode, put_RingMode, put_RingMode method [TAPI 2.2], put_RingMode method [TAPI 2.2],ITPhone interface, tapi3.itphone_put_ringmode, tapi3if/ITPhone::put_RingMode
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: TERMINAL_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Tapi3.dll
api_name:
-	ITPhone.put_RingMode
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITPhone::put_RingMode


## -description


The 
<b>put_RingMode</b> method requests that the phone change its ring mode.

The application must call 
<a href="https://msdn.microsoft.com/d9efe2f7-3628-4e1f-b554-a6889d82a973">ITPhone::Open</a> before invoking this method; otherwise, the invocation fails.


## -parameters




### -param lRingMode [in]

Ring mode.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/94dff33c-67a1-4df8-9ef5-2b6524438f6f">ITPhone</a>



<a href="https://msdn.microsoft.com/55f6a75c-dffb-46e7-8679-70c7d59ff5b4">get_RingMode</a>
 

 
