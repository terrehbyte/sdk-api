---
UID: NF:tapi3if.ITAddress.get_AddressName
title: ITAddress::get_AddressName
author: windows-driver-content
description: The get_AddressName method gets the displayable name of the address.
old-location: tapi3\itaddress_get_addressname.htm
old-project: Tapi
ms.assetid: cb26dcf5-0192-4156-914b-9aa6e76a2bd2
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITAddress interface [TAPI 2.2],get_AddressName method, ITAddress.get_AddressName, ITAddress::get_AddressName, _tapi3_itaddress_get_addressname, get_AddressName, get_AddressName method [TAPI 2.2], get_AddressName method [TAPI 2.2],ITAddress interface, tapi3.itaddress_get_addressname, tapi3if/ITAddress::get_AddressName
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
-	ITAddress.get_AddressName
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITAddress::get_AddressName


## -description


The 
<b>get_AddressName</b> method gets the displayable name of the address.


## -parameters




### -param ppName [out]

Pointer to <b>BSTR</b> containing a displayable address name.


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
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
The <i>ppName</i> parameter is not a valid pointer.

</td>
</tr>
</table>
 




## -remarks



The application must use 
<a href="8f230ee3-5f6e-4cb9-a910-9c90b754dcd3">SysFreeString</a> to free the memory allocated for the <i>ppName</i> parameter.
			




## -see-also




<a href="https://msdn.microsoft.com/ab6db262-f99e-4027-9525-7597fcf02e72">Address Object</a>



<a href="https://msdn.microsoft.com/93f2e4cf-013e-4064-88d5-69fddd458274">ITAddress</a>
 

 
