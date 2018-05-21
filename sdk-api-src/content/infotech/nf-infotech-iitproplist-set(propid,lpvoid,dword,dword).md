---
UID: NF:infotech.IITPropList.Set(PROPID,LPVOID,DWORD,DWORD)
title: IITPropList::Set(PROPID,LPVOID,DWORD,DWORD)
author: windows-driver-content
description: Sets a property to a given value or deletes a property from the list.
old-location: htmlhelp\iitproplist_set2.htm
old-project: htmlhelp
ms.assetid: VS|htmlhelp|~\html\refiitproplistsetpointertobuffer.htm
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: IITPropList interface [HTML Help Workshop],Set method, IITPropList.Set, IITPropList.Set(PROPID,LPVOID,DWORD,DWORD), IITPropList::Set, IITPropList::Set(PROPID,LPVOID,DWORD,DWORD), PROP_ADD, PROP_DELETE, PROP_UPDATE, Set, Set method [HTML Help Workshop], Set method [HTML Help Workshop],IITPropList interface, htmlhelp.iitproplist_set2, infotech/IITPropList::Set, refIITPropListSetPointerToBuffer
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
-	IITPropList.Set
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IITPropList::Set(PROPID,LPVOID,DWORD,DWORD)


## -description


Sets a property to a given value or deletes a property from the list.




## -parameters




### -param PropID [in]

ID of the property to set.




### -param lpvData [in]

Pointer to the buffer containing data.




### -param cbData [in]

Length of the buffer.




### -param dwOperation [in]

The operation you want to perform. Can be any of the following flags: 



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="PROP_ADD"></a><a id="prop_add"></a><dl>
<dt><b>PROP_ADD</b></dt>
</dl>
</td>
<td width="60%">
Add property to list

</td>
</tr>
<tr>
<td width="40%"><a id="PROP_DELETE"></a><a id="prop_delete"></a><dl>
<dt><b>PROP_DELETE</b></dt>
</dl>
</td>
<td width="60%">
Remove property from list

</td>
</tr>
<tr>
<td width="40%"><a id="PROP_UPDATE"></a><a id="prop_update"></a><dl>
<dt><b>PROP_UPDATE</b></dt>
</dl>
</td>
<td width="60%">
Update property in list

</td>
</tr>
</table>
 


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
The property list was successfully set.



</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_DUPLICATE</b></dt>
</dl>
</td>
<td width="60%">
The property already exists in the list (applies to adding).



</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Memory could not be allocated when adding a property.



</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTEXIST</b></dt>
</dl>
</td>
<td width="60%">
The property does not exist (applies to deleting and updating).



</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOTIMPL</b></dt>
</dl>
</td>
<td width="60%">
The specified operation is not available.

</td>
</tr>
</table>
 




## -remarks



Use this method to set properties stored in a buffer.






## -see-also




<a href="https://msdn.microsoft.com/09200749-bd1d-4266-895e-29e21525bac2">IITPropList</a>
 

 
