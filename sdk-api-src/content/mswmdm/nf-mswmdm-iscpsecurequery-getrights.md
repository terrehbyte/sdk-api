---
UID: NF:mswmdm.ISCPSecureQuery.GetRights
title: ISCPSecureQuery::GetRights
author: windows-sdk-content
description: The GetRights method retrieves rights information for the current piece of content. Rights are file-specific.
old-location: wmdm\iscpsecurequery_getrights.htm
old-project: WMDM
ms.assetid: 3d9991f4-ce20-45c4-a408-d7a846b019ef
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: GetRights, GetRights method [windows Media Device Manager], GetRights method [windows Media Device Manager],ISCPSecureQuery interface, ISCPSecureQuery interface [windows Media Device Manager],GetRights method, ISCPSecureQuery.GetRights, ISCPSecureQuery::GetRights, ISCPSecureQueryGetRights, mswmdm/ISCPSecureQuery::GetRights, wmdm.iscpsecurequery_getrights
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: mswmdm.h
req.include-header: 
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
req.typenames: MSVidCtlStateList
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	mssachlp.lib
-	mssachlp.dll
api_name:
-	ISCPSecureQuery.GetRights
product: Windows
targetos: Windows
req.lib: Mssachlp.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ISCPSecureQuery::GetRights


## -description



The <b>GetRights</b> method retrieves rights information for the current piece of content. Rights are file-specific.




## -parameters




### -param pData [in]

Pointer to data requested by <a href="https://msdn.microsoft.com/c4ed4da1-9378-4c35-8f03-b028e37c1707">GetDataDemands</a>. This parameter must be included in the input message authentication code and must be encrypted.


### -param dwSize [in]

Number of bytes of data in the <i>pData</i> buffer. This parameter must be included in the input message authentication code.


### -param pbSPSessionKey [in]

Pointer to an array of bytes containing the session key for securing communication with the service provider to which <i>pStgGlobals</i> points. This parameter must be included in the input message authentication code and must be encrypted.


### -param dwSessionKeyLen [in]

Length of the byte array to which <i>pbSPSessionKey</i> points. This parameter must be included in the input message authentication code.


### -param pStgGlobals [in]

Pointer to an <a href="https://msdn.microsoft.com/fe164271-58f0-4b28-a200-6b15f8b42d36">IWMDMStorageGlobals</a> interface on the root storage of the media or device to or from which the file is being transferred.


### -param ppRights [out]

Pointer to an array of <a href="https://msdn.microsoft.com/1be9167b-0d20-4a17-a42b-9696ada2b539">WMDMRIGHTS</a> structures containing the rights information for this object. The array is allocated by this method and must be freed using <b>CoTaskMemFree</b>. This parameter is included in the output message authentication code.


### -param pnRightsCount [out]

Number of <b>WMDMRIGHTS</b> structures in the <i>ppRights</i> array. This parameter is included in the output message authentication code.


### -param abMac [in, out]

Array of eight bytes containing the message authentication code for the parameter data of this method. (WMDM_MAC_LENGTH is defined as 8.)


## -returns



If the method succeeds, it returns S_OK. If it fails, it returns an <b>HRESULT</b> error code.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WMDM_E_CALL_OUT_OF_SEQUENCE</b></dt>
</dl>
</td>
<td width="60%">
This method was called out of sequence. <b>GetDataDemands</b> and then <a href="https://msdn.microsoft.com/e12d8b55-5600-4178-8b2b-8afe8ade6818">ExamineData</a> must be called first, in that order.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WMDM_E_MAC_CHECK_FAILED</b></dt>
</dl>
</td>
<td width="60%">
The message authentication code is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>WMDM_E_NORIGHTS</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have the rights required to perform the requested operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
A parameter is invalid or is a <b>NULL</b> pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
An unspecified error occurred.

</td>
</tr>
</table>
 




## -remarks



This method must not be called until <b>GetDataDemands</b> and then <b>ExamineData</b> have been called, in that order.




## -see-also




<a href="https://msdn.microsoft.com/d5f96629-26a1-4e83-a6a8-2d60c463f407">ISCPSecureQuery Interface</a>



<a href="https://msdn.microsoft.com/fe164271-58f0-4b28-a200-6b15f8b42d36">IWMDMStorageGlobals Interface</a>



<a href="https://msdn.microsoft.com/1be9167b-0d20-4a17-a42b-9696ada2b539">WMDMRIGHTS</a>
 

 
