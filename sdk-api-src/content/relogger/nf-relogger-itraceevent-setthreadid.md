---
UID: NF:relogger.ITraceEvent.SetThreadId
title: ITraceEvent::SetThreadId
author: windows-sdk-content
description: Sets the identifier of a thread that generates an event.
old-location: etw\ievent_setthreadid.htm
old-project: ETW
ms.assetid: 9f5d293e-da87-4b83-9407-fc4179a42a46
ms.author: windowssdkdev
ms.date: 05/29/2018
ms.keywords: ITraceEvent interface [ETW],SetThreadId method, ITraceEvent.SetThreadId, ITraceEvent::SetThreadId, SetThreadId, SetThreadId method [ETW], SetThreadId method [ETW],ITraceEvent interface, etw.ievent_setthreadid, relogger/ITraceEvent::SetThreadId
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: relogger.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Relogger.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: RECO_RANGE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Relogger.h
api_name:
-	ITraceEvent.SetThreadId
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ITraceEvent::SetThreadId


## -description


The <b>SetThreadId</b> method sets the identifier of a thread that generates an event.


## -parameters




### -param ThreadId [in]

Type: <b>ULONG</b>

Identifier of the thread that generates the event.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/29b6f72a-ae81-4292-a023-a4bab16ae143">ITraceEvent</a>
 

 
