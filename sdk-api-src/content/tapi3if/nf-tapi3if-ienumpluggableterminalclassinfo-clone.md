---
UID: NF:tapi3if.IEnumPluggableTerminalClassInfo.Clone
title: IEnumPluggableTerminalClassInfo::Clone
author: windows-driver-content
description: The Clone method creates another enumerator that contains the same enumeration state as the current one. This method is hidden from Visual Basic and scripting languages.
old-location: tapi3\ienumpluggableterminalclassinfo_clone.htm
old-project: Tapi
ms.assetid: cc5fb452-c166-46dc-a529-be08924b15a4
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: Clone, Clone method [TAPI 2.2], Clone method [TAPI 2.2],IEnumPluggableTerminalClassInfo interface, IEnumPluggableTerminalClassInfo interface [TAPI 2.2],Clone method, IEnumPluggableTerminalClassInfo.Clone, IEnumPluggableTerminalClassInfo::Clone, _tapi3_ienumpluggableterminalclassinfo_clone, tapi3.ienumpluggableterminalclassinfo_clone, tapi3if/IEnumPluggableTerminalClassInfo::Clone
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
-	IEnumPluggableTerminalClassInfo.Clone
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# IEnumPluggableTerminalClassInfo::Clone


## -description


The 
<b>Clone</b> method creates another enumerator that contains the same enumeration state as the current one. This method is hidden from Visual Basic and scripting languages.


## -parameters




### -param ppEnum [out]

Pointer to new 
<a href="https://msdn.microsoft.com/72c0db41-8391-4923-8961-6aefce9886c4">IEnumPluggableTerminalClassInfo</a> interface.


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
The <i>ppEnum</i> parameter is not a valid pointer.

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
<dt><b>E_UNEXPECTED</b></dt>
</dl>
</td>
<td width="60%">
The method failed for unknown reasons.

</td>
</tr>
</table>
 




## -remarks



TAPI calls the <a href="_com_iunknown_addref">AddRef</a> method on the 
<a href="https://msdn.microsoft.com/72c0db41-8391-4923-8961-6aefce9886c4">IEnumPluggableTerminalClassInfo</a> interface returned by <b>IEnumPluggableTerminalClassInfo::Clone</b>. The application must call <a href="_com_iunknown_release">Release</a> on the 
<b>IEnumPluggableTerminalClassInfo</b> interface to free resources associated with it.




## -see-also




<a href="https://msdn.microsoft.com/72c0db41-8391-4923-8961-6aefce9886c4">IEnumPluggableTerminalClassInfo</a>



<a href="https://msdn.microsoft.com/2a16d33c-2d87-4172-a5ff-33ff62e96615">Terminal Class</a>
 

 
