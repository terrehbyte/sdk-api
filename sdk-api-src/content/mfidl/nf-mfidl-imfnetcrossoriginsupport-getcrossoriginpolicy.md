---
UID: NF:mfidl.IMFNetCrossOriginSupport.GetCrossOriginPolicy
title: IMFNetCrossOriginSupport::GetCrossOriginPolicy
author: windows-driver-content
description: Returns the client's current cross-origin policy to apply to the download session.
old-location: mf\imfnetcrossoriginsupport_getcrossoriginpolicy.htm
old-project: medfound
ms.assetid: B74FA337-014E-4A5C-83CD-26C563E9BBD4
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: GetCrossOriginPolicy, GetCrossOriginPolicy method [Media Foundation], GetCrossOriginPolicy method [Media Foundation],IMFNetCrossOriginSupport interface, IMFNetCrossOriginSupport interface [Media Foundation],GetCrossOriginPolicy method, IMFNetCrossOriginSupport.GetCrossOriginPolicy, IMFNetCrossOriginSupport::GetCrossOriginPolicy, mf.imfnetcrossoriginsupport_getcrossoriginpolicy, mfidl/IMFNetCrossOriginSupport::GetCrossOriginPolicy
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
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
-	mfuuid.lib
-	mfuuid.dll
api_name:
-	IMFNetCrossOriginSupport.GetCrossOriginPolicy
product: Windows
targetos: Windows
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IMFNetCrossOriginSupport::GetCrossOriginPolicy


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Returns the client's current cross-origin policy to apply to the download session.


## -parameters




### -param pPolicy [out]

A value indicating the client's current cross-origin policy to apply to the download session.


## -returns



Returns S_OK upon successful completion.




## -see-also




<a href="https://msdn.microsoft.com/239E5731-4425-46D4-AFEC-F3E59258B1DF">IMFNetCrossOriginSupport</a>
 

 
