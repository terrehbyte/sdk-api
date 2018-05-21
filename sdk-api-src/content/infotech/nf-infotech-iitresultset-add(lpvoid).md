---
UID: NF:infotech.IITResultSet.Add(LPVOID)
title: IITResultSet::Add(LPVOID)
author: windows-driver-content
description: Adds columns to result set, given a header containing pairs of property ID followed by property type.
old-location: htmlhelp\iitresultset_add1.htm
old-project: htmlhelp
ms.assetid: VS|htmlhelp|~\html\refiitresultsetadd.htm
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: Add, Add method [HTML Help Workshop], Add method [HTML Help Workshop],IITResultSet interface, IITResultSet interface [HTML Help Workshop],Add method, IITResultSet.Add, IITResultSet.Add(LPVOID), IITResultSet::Add, IITResultSet::Add(LPVOID), htmlhelp.iitresultset_add1, infotech/IITResultSet::Add, refIITResultSetAdd
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: infotech.h
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
req.typenames: POLICY_ELEMENT, *PPOLICY_ELEMENT
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Infotech.h
api_name:
-	IITResultSet.Add
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IITResultSet::Add(LPVOID)


## -description


Adds columns to result set, given a header containing pairs of property ID followed by property type.




## -parameters




### -param lpvHdr [in]

Buffer containing property ID/property pairs.




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
The columns were successfully added.



</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/e77b1489-a883-4f98-acb0-b998cbe3d46e">IITResultSet</a>
 

 
