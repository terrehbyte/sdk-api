---
UID: NF:gdiplusstringformat.StringFormat.GetLastStatus
title: StringFormat::GetLastStatus
author: windows-driver-content
description: The StringFormat::GetLastStatus method returns a value that indicates the nature of this StringFormat object's most recent method failure.
old-location: gdiplus\_gdiplus_CLASS_StringFormat_GetLastStatus_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\stringformatclass\stringformatmethods\getlaststatus_15.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetLastStatus, GetLastStatus method [GDI+], GetLastStatus method [GDI+],StringFormat class, StringFormat class [GDI+],GetLastStatus method, StringFormat.GetLastStatus, StringFormat::GetLastStatus, _gdiplus_CLASS_StringFormat_GetLastStatus_, gdiplus._gdiplus_CLASS_StringFormat_GetLastStatus_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusstringformat.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Gdiplus.dll
api_name:
-	StringFormat.GetLastStatus
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# StringFormat::GetLastStatus


## -description


The <b>StringFormat::GetLastStatus</b> method returns a value that indicates the nature of this 
			<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object's most recent method failure.


## -parameters






## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

The <b>StringFormat::GetLastStatus</b> method returns an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If no methods invoked on this 
						<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object have failed since the previous call to <b>StringFormat::GetLastStatus</b>, then <b>StringFormat::GetLastStatus</b> returns Ok.

If at least one method invoked on this 
						<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object has failed since the previous call to <b>StringFormat::GetLastStatus</b>, then <b>StringFormat::GetLastStatus</b> returns a value that indicates the nature of the most recent failure.




## -remarks



You can call <b>StringFormat::GetLastStatus</b> immediately after constructing a 
				<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object to determine whether the constructor succeeded.

The first time you call the <b>StringFormat::GetLastStatus</b> method of a 
				<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object, it returns Ok if the constructor succeeded and all methods invoked so far on the 
				<b>StringFormat</b> object succeeded. Otherwise, it returns a value that indicates the nature of the most recent failure.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a> object, calls two 
						<b>StringFormat</b> methods, and then checks the status to see if an error occurred during the construction or either of the method calls.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>StringFormat stringFormat;
stringFormat.SetAlignment(StringAlignmentCenter);
HotkeyPrefix hotkeyPrefix = stringFormat.GetHotkeyPrefix();

if (stringFormat.GetLastStatus() == Ok)
{
   // There have been no errors since the previous call to GetLastStatus.
}
else
{
   // An error occurred since the previous call to GetLastStatus.
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/2d7af5fe-f3e9-4db3-90a5-4e623d9ce773">StringFormat</a>



<a href="https://msdn.microsoft.com/9bbddab0-46b1-49db-86c1-cf9086692958">StringFormatFlags</a>
 

 
