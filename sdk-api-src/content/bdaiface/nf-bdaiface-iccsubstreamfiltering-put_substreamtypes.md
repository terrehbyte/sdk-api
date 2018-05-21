---
UID: NF:bdaiface.ICCSubStreamFiltering.put_SubstreamTypes
title: ICCSubStreamFiltering::put_SubstreamTypes
author: windows-driver-content
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
old-location: mstv\iccsubstreamfiltering_put_substreamtypes.htm
old-project: mstv
ms.assetid: 45db472d-cffc-42d1-8270-3a0db72bdc2c
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: ICCSubStreamFiltering interface [Microsoft TV Technologies],put_SubstreamTypes method, ICCSubStreamFiltering.put_SubstreamTypes, ICCSubStreamFiltering::put_SubstreamTypes, ICCSubStreamFilteringput_SubstreamTypes, bdaiface/ICCSubStreamFiltering::put_SubstreamTypes, mstv.iccsubstreamfiltering_put_substreamtypes, put_SubstreamTypes, put_SubstreamTypes method [Microsoft TV Technologies], put_SubstreamTypes method [Microsoft TV Technologies],ICCSubStreamFiltering interface
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: bdaiface.h
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
req.typenames: UICloseReasonType
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	bdaiface.h
api_name:
-	ICCSubStreamFiltering.put_SubstreamTypes
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# ICCSubStreamFiltering::put_SubstreamTypes


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>get_SubstreamTypes</b> method sets the closed captioning services the pin will deliver.


## -parameters




### -param Types [in]

Bitwise OR of flags that specify the closed captioning services. For a list of flags, see <a href="https://msdn.microsoft.com/1a55a9b1-6784-4a29-93aa-95aadaf6fb7e">KS_CC_SUBSTREAM Constants</a>. Any services that are not selected are simply dropped.


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
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/2de6796d-beb3-4611-a559-449fe21193a6">ICCSubStreamFiltering Interface</a>
 

 
