---
UID: NF:infotech.IITResultSet.Add(PROPID,LPCWSTR,PRIORITY)
title: IITResultSet::Add(PROPID,LPCWSTR,PRIORITY)
author: windows-driver-content
description: Adds a column to the result set.
old-location: htmlhelp\iitresultset_add3.htm
old-project: htmlhelp
ms.assetid: VS|htmlhelp|~\html\refiitresultsetaddstring.htm
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: Add, Add method [HTML Help Workshop], Add method [HTML Help Workshop],IITResultSet interface, IITResultSet interface [HTML Help Workshop],Add method, IITResultSet.Add, IITResultSet.Add(PROPID,LPCWSTR,PRIORITY), IITResultSet::Add, IITResultSet::Add(PROPID,LPCWSTR,PRIORITY), htmlhelp.iitresultset_add3, infotech/IITResultSet::Add, refIITResultSetAddString
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

# IITResultSet::Add(PROPID,LPCWSTR,PRIORITY)


## -description


Adds a column to the result set.




## -parameters




### -param PropID [in]

Property ID associated with column.




### -param lpszwDefault [in]

Default value of string.




### -param Priority [in]

Download priority of column (PRIORITY_LOW, PRIORITY_NORMAL, or PRIORITY_HIGH). 


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
The column was successfully added. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Memory allocation failed.



</td>
</tr>
</table>
 




## -remarks



This method is used to add a column for string properties. 






## -see-also




<a href="https://msdn.microsoft.com/e77b1489-a883-4f98-acb0-b998cbe3d46e">IITResultSet</a>
 

 
