---
UID: NF:infotech.IITResultSet.Add(PROPID,LPVOID,DWORD,PRIORITY)
title: IITResultSet::Add(PROPID,LPVOID,DWORD,PRIORITY)
author: windows-driver-content
description: Adds a column to the result set.
old-location: htmlhelp\iitresultset_add2.htm
old-project: htmlhelp
ms.assetid: VS|htmlhelp|~\html\refiitresultsetaddbuffer.htm
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: Add, Add method [HTML Help Workshop], Add method [HTML Help Workshop],IITResultSet interface, IITResultSet interface [HTML Help Workshop],Add method, IITResultSet.Add, IITResultSet.Add(PROPID,LPVOID,DWORD,PRIORITY), IITResultSet::Add, IITResultSet::Add(PROPID,LPVOID,DWORD,PRIORITY), htmlhelp.iitresultset_add2, infotech/IITResultSet::Add, refIITResultSetAddBuffer
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

# IITResultSet::Add(PROPID,LPVOID,DWORD,PRIORITY)


## -description


Adds a column to the result set.




## -parameters




### -param PropID [in]

Property ID associated with column.




### -param lpvDefaultData [in]

Buffer containing default value of data.




### -param cbData [in]

Buffer size.




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



This method is used to add a column for pointer properties. 






## -see-also




<a href="https://msdn.microsoft.com/e77b1489-a883-4f98-acb0-b998cbe3d46e">IITResultSet</a>
 

 
