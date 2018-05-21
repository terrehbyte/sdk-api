---
UID: NN:mfidl.IMFHttpDownloadSessionProvider
title: IMFHttpDownloadSessionProvider
author: windows-driver-content
description: Applications implement this interface in order to provide custom a custom HTTP or HTTPS download implementation.
old-location: mf\imfhttpdownloadsessionprovider.htm
old-project: medfound
ms.assetid: 4A3A96FB-A7C5-40BB-AB8F-12A7F00FDCD1
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: IMFHttpDownloadSessionProvider, IMFHttpDownloadSessionProvider interface [Media Foundation], IMFHttpDownloadSessionProvider interface [Media Foundation],described, mf.imfhttpdownloadsessionprovider, mfidl/IMFHttpDownloadSessionProvider
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
-	IMFHttpDownloadSessionProvider
product: Windows
targetos: Windows
req.lib: Mfplat.lib; Mfplat.dll
req.dll: Mfplat.dll
req.irql: 
req.product: GDI+ 1.1
---

# IMFHttpDownloadSessionProvider interface


## -description


Applications implement this interface in order to provide custom a custom HTTP or HTTPS download implementation. Use the <a href="https://msdn.microsoft.com/079c61c5-7a29-4411-840e-9349190726ac">IMFSourceResolver</a> interface to register the provider. For more information, see <a href="https://msdn.microsoft.com/94e2a411-96b8-4506-8491-78f4f5f286ce">Using the Source Resolver</a>. Once registered, the Microsoft Media Foundation will invoke the <a href="https://msdn.microsoft.com/D9DAE789-1C0E-42B4-87B6-593D3B67FE1F">CreateHttpDownloadSession</a> method of the provider  implementation to open HTTP or HTTPS URLs instead of using the default implementation.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMFHttpDownloadSessionProvider</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMFHttpDownloadSessionProvider</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMFHttpDownloadSessionProvider</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/D9DAE789-1C0E-42B4-87B6-593D3B67FE1F">CreateHttpDownloadSession</a>
</td>
<td align="left" width="63%">
Called by the Microsoft Media Foundation to open HTTP or HTTPS URLs instead of using the default implementation.

</td>
</tr>
</table> 
