---
UID: NF:mfidl.IMFHttpDownloadRequest.BeginSendRequest
title: IMFHttpDownloadRequest::BeginSendRequest
author: windows-driver-content
description: Invoked by Microsoft Media Foundation to send a HTTP or HTTPS request.
old-location: mf\imfhttpdownloadrequest_beginsendrequest.htm
old-project: medfound
ms.assetid: 38025B19-146A-4050-9BD2-2CF974729FE3
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: BeginSendRequest, BeginSendRequest method [Media Foundation], BeginSendRequest method [Media Foundation],IMFHttpDownloadRequest interface, IMFHttpDownloadRequest interface [Media Foundation],BeginSendRequest method, IMFHttpDownloadRequest.BeginSendRequest, IMFHttpDownloadRequest::BeginSendRequest, mf.imfhttpdownloadrequest_beginsendrequest, mfidl/IMFHttpDownloadRequest::BeginSendRequest
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1703 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: MF_URL_TRUST_STATUS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	mfplat.lib
-	mfplat.dll
-	mfplat.dll
-	mfplat.dll.dll
api_name:
-	IMFHttpDownloadRequest.BeginSendRequest
product: Windows
targetos: Windows
req.lib: Mfplat.lib; Mfplat.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IMFHttpDownloadRequest::BeginSendRequest


## -description


Invoked by Microsoft Media Foundation to send a HTTP or HTTPS request


## -parameters




### -param pbPayload [in]

Pointer to a buffer that contains the message payload to send in the request. This parameter is used for POST requests. GET requests do not carry a message payload and therefore <i>pbPayload</i> is NULL.


### -param cbPayload [in]

The size of the <i>pbPayload</i> buffer, in bytes.


### -param pCallback [in]

Pointer to the <a href="https://msdn.microsoft.com/7edff985-da59-4cc0-96de-1a92e03a7d41">IMFAsyncCallback</a> interface of a callback object that is implemented by Microsoft Media Foundation.


### -param punkState

Pointer to the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface of a state object, defined by Microsoft Media Foundation. This parameter can be NULL.


## -returns




            The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.
          

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">

                Successfully started the asynchronous operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">

                There is insufficient memory to complete the operation.

</td>
</tr>
</table>
 




## -remarks



The implementation of <b>BeginWrite</b> does not need to make a private copy of the memory pointed to by <i>pbPayload</i>, as Microsoft Media Foundation will not reallocate, free, or write to the buffer while an asynchronous write is still pending.




## -see-also




<a href="https://msdn.microsoft.com/A8A37C2F-A662-4FDA-95F6-43D96A8471A8">IMFHttpDownloadRequest</a>
 

 
