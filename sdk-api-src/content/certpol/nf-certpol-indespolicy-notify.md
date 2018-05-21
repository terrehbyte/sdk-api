---
UID: NF:certpol.INDESPolicy.Notify
title: INDESPolicy::Notify
author: windows-driver-content
description: Notifies the plug-in of the transaction status of the SCEP certificate request.
old-location: security\indespolicy_notify.htm
old-project: SecCrypto
ms.assetid: dcb1c006-c709-4879-a9bf-8d441d26db8d
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: INDESPolicy interface [Security],Notify method, INDESPolicy.Notify, INDESPolicy::Notify, Notify, Notify method [Security], Notify method [Security],INDESPolicy interface, certpol/INDESPolicy::Notify, security.indespolicy_notify
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: certpol.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certpol.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: X509SCEPFailInfo
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	certpol.h
api_name:
-	INDESPolicy.Notify
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# INDESPolicy::Notify


## -description


Notifies the plug-in of the transaction status of the SCEP certificate request.


## -parameters




### -param pwszChallenge [in]

The authentication and authorization SCEP challenge password for the user.


### -param pwszTransactionId [in]

The SCEP request transaction ID.


### -param disposition [in]

The disposition of the transaction.


### -param lastHResult [in]

The <b>HRESULT</b> of the last operation.


### -param pctbIssuedCertEncoded [in]

The requested certificate, if issued.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/9ed31493-832a-4f66-bb95-02ef1ad7ca15">INDESPolicy</a>
 

 
