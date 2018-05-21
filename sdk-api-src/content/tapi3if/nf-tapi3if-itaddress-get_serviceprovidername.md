---
UID: NF:tapi3if.ITAddress.get_ServiceProviderName
title: ITAddress::get_ServiceProviderName
author: windows-driver-content
description: The get_ServiceProviderName method gets the name of the Telephony Service Provider (TSP) that supports this address:\_for example, Unimdm.tsp for the Unimodem service provider or H323.tsp for the H323 service provider.
old-location: tapi3\itaddress_get_serviceprovidername.htm
old-project: Tapi
ms.assetid: fa49d256-58e0-4d7e-a121-387a3a704519
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITAddress interface [TAPI 2.2],get_ServiceProviderName method, ITAddress.get_ServiceProviderName, ITAddress::get_ServiceProviderName, _tapi3_itaddress_get_serviceprovidername, get_ServiceProviderName, get_ServiceProviderName method [TAPI 2.2], get_ServiceProviderName method [TAPI 2.2],ITAddress interface, tapi3.itaddress_get_serviceprovidername, tapi3if/ITAddress::get_ServiceProviderName
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
-	ITAddress.get_ServiceProviderName
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITAddress::get_ServiceProviderName


## -description


The 
<b>get_ServiceProviderName</b> method gets the name of the Telephony Service Provider (TSP) that supports this address: for example, Unimdm.tsp for the Unimodem service provider or H323.tsp for the H323 service provider.


## -parameters




### -param ppName [out]

Pointer to <b>BSTR</b> containing the service provider name.


## -returns



This method can return one of these values.

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
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppName</i> parameter is not a valid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TAPI_E_NODRIVER</b></dt>
</dl>
</td>
<td width="60%">
No service provider was found that supports the current address.

</td>
</tr>
</table>
 




## -remarks



The application must use 
<a href="8f230ee3-5f6e-4cb9-a910-9c90b754dcd3">SysFreeString</a> to free the memory allocated for the <i>ppName</i> parameter.
			

You can retrieve the name of the provider in a TSP-dependent format using 
<a href="https://msdn.microsoft.com/9ec4c25e-700b-4aed-97ff-e7cb420fdf96">ITAddressCapabilities::get_AddressCapabilityString</a> with <i>AddressCapString</i> set to ACS_PROVIDERSPECIFIC, which returns the string found in the <b>dwProviderInfoOffset</b> member of the TAPI 2.<i>x</i>
<a href="https://msdn.microsoft.com/83e38453-bb93-4cc5-923f-d0cd2898350a">LINEDEVCAPS</a> structure.




## -see-also




<a href="https://msdn.microsoft.com/ab6db262-f99e-4027-9525-7597fcf02e72">Address Object</a>



<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a>



<a href="https://msdn.microsoft.com/9ec4c25e-700b-4aed-97ff-e7cb420fdf96">ITAddressCapabilities::get_AddressCapabilityString</a>



<a href="https://msdn.microsoft.com/83e38453-bb93-4cc5-923f-d0cd2898350a">LINEDEVCAPS</a>
 

 
