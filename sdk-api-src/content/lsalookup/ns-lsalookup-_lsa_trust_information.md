---
UID: NS:lsalookup._LSA_TRUST_INFORMATION
title: "_LSA_TRUST_INFORMATION"
author: windows-driver-content
description: Identifies a domain.
old-location: security\lsa_trust_information.htm
old-project: SecMgmt
ms.assetid: 2b5e6f79-b97a-4018-a45a-37c300c3dc0d
ms.author: windowsdriverdev
ms.date: 5/9/2018
ms.keywords: "*PLSA_TRUST_INFORMATION, LSA_TRUST_INFORMATION, LSA_TRUST_INFORMATION structure [Security], PLSA_TRUST_INFORMATION, PLSA_TRUST_INFORMATION structure pointer [Security], _LSA_TRUST_INFORMATION, _lsa_lsa_trust_information, lsalookup/LSA_TRUST_INFORMATION, lsalookup/PLSA_TRUST_INFORMATION, security.lsa_trust_information"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: lsalookup.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: LSA_TRUST_INFORMATION, *PLSA_TRUST_INFORMATION
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	lsalookup.h
api_name:
-	LSA_TRUST_INFORMATION
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# _LSA_TRUST_INFORMATION structure


## -description


The <b>LSA_TRUST_INFORMATION</b> structure identifies a domain.


## -struct-fields




### -field Name

An 
<a href="https://msdn.microsoft.com/9e1cf20f-01f9-4813-bf95-e47c5d57dcdc">LSA_UNICODE_STRING</a> structure that contains the name of the domain.


### -field Sid

Pointer to the SID of the domain.


## -see-also




<a href="https://msdn.microsoft.com/ddf0afcb-7ec4-42ed-bf40-38ef33f33a0c">LSA_REFERENCED_DOMAIN_LIST</a>



<a href="https://msdn.microsoft.com/9e1cf20f-01f9-4813-bf95-e47c5d57dcdc">LSA_UNICODE_STRING</a>
 

 
