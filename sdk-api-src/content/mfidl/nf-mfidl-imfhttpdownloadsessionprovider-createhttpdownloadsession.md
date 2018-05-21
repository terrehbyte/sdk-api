---
UID: NF:mfidl.IMFHttpDownloadSessionProvider.CreateHttpDownloadSession
title: IMFHttpDownloadSessionProvider::CreateHttpDownloadSession
author: windows-driver-content
description: Called by the Microsoft Media Foundation to open HTTP or HTTPS URLs instead of using the default implementation.
old-location: mf\imfhttpdownloadsessionprovider_createhttpdownloadsession.htm
old-project: medfound
ms.assetid: D9DAE789-1C0E-42B4-87B6-593D3B67FE1F
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: CreateHttpDownloadSession, CreateHttpDownloadSession method [Media Foundation], CreateHttpDownloadSession method [Media Foundation],IMFHttpDownloadSessionProvider interface, IMFHttpDownloadSessionProvider interface [Media Foundation],CreateHttpDownloadSession method, IMFHttpDownloadSessionProvider.CreateHttpDownloadSession, IMFHttpDownloadSessionProvider::CreateHttpDownloadSession, mf.imfhttpdownloadsessionprovider_createhttpdownloadsession, mfidl/IMFHttpDownloadSessionProvider::CreateHttpDownloadSession
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
-	IMFHttpDownloadSessionProvider.CreateHttpDownloadSession
product: Windows
targetos: Windows
req.lib: Mfplat.lib; Mfplat.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IMFHttpDownloadSessionProvider::CreateHttpDownloadSession


## -description


Called by the Microsoft Media Foundation to open HTTP or HTTPS URLs instead of using the default implementation.


## -parameters




### -param wszScheme [in]

The name of the protocol to for which an <a href="https://msdn.microsoft.com/048B2922-3B77-4F2D-9437-0FA54F94C67E">IMFHttpDownloadSession</a> is being requested.  Microsoft Media Foundation specifies the protocol scheme of the URL that the application provided the Media Foundation Source Resolver. Valid values include “http” for HTTP, and “https” for HTTPS. URL scheme names are generally not case-sensitive. 


### -param ppDownloadSession [out]

On successful execution, the parameter is set to a pointer to an <a href="https://msdn.microsoft.com/048B2922-3B77-4F2D-9437-0FA54F94C67E">IMFHttpDownloadSession</a> interface. The returned interface is used by Microsoft Media Foundation to open a single HTTP or HTTPS URL. 


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

                Successfully created the <a href="https://msdn.microsoft.com/048B2922-3B77-4F2D-9437-0FA54F94C67E">IMFHttpDownloadSession</a> object.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">

                The value specified for the <i>wszScheme</i> parameter is incorrect.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">

                The <i>ppDownloadSession</i> parameter is an invalid pointer.

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



Specifying “https” as the value of <i>wszScheme</i> does not imply that HTTPS will be used for a particular request, as that is specified on a per-request basis in <a href="https://msdn.microsoft.com/111A075A-82A7-4607-9359-37B2DA97AFC5">IMFhttpDownloadSession::CreateRequest</a>.




## -see-also




<a href="https://msdn.microsoft.com/4A3A96FB-A7C5-40BB-AB8F-12A7F00FDCD1">IMFHttpDownloadSessionProvider</a>
 

 
