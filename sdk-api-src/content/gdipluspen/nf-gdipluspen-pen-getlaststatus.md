---
UID: NF:gdipluspen.Pen.GetLastStatus
title: Pen::GetLastStatus
author: windows-driver-content
description: The Pen::GetLastStatus method returns a value that indicates the nature of this Pen object's most recent method failure.
old-location: gdiplus\_gdiplus_CLASS_Pen_GetLastStatus_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\penclass\penmethods\getlaststatus_88.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetLastStatus, GetLastStatus method [GDI+], GetLastStatus method [GDI+],Pen class, Pen class [GDI+],GetLastStatus method, Pen.GetLastStatus, Pen::GetLastStatus, _gdiplus_CLASS_Pen_GetLastStatus_, gdiplus._gdiplus_CLASS_Pen_GetLastStatus_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspen.h
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
req.typenames: WmfPlaceableFileHeader
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Gdiplus.dll
api_name:
-	Pen.GetLastStatus
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Pen::GetLastStatus


## -description


The <b>Pen::GetLastStatus</b> method returns a value that indicates the nature of this 
			<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object's most recent method failure.


## -parameters






## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

The <b>Pen::GetLastStatus</b> method returns an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If no methods invoked on this 
						<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object have failed since the previous call to <b>Pen::GetLastStatus</b>, then <b>Pen::GetLastStatus</b> returns <b>Ok</b>.

If at least one method invoked on this 
						<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object has failed since the previous call to <b>Pen::GetLastStatus</b>, then <b>Pen::GetLastStatus</b> returns a value that indicates the nature of the most recent failure.




## -remarks



You can call <b>Pen::GetLastStatus</b> immediately after constructing a 
				<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object to determine whether the constructor succeeded.

The first time you call the <b>Pen::GetLastStatus</b> method of a 
				<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object, it returns <b>Ok</b> if the constructor succeeded and all methods invoked so far on the 
				<b>Pen</b> object succeeded. Otherwise, it returns a value that indicates the nature of the most recent failure.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object, sets the dash style, and draws a dashed line. The code then checks the status of the method that sets the dash style for the pen.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_GetLastStatus(HDC hdc)
{
   Graphics graphics(hdc);
   
   // Create a pen.
   Pen pen(Color(255, 255, 0, 0), 5);

   // Set the dash style, and draw a dashed line.
   pen.SetDashStyle(DashStyleDash);
   graphics.DrawLine(&amp;pen, 0, 0, 200, 100);

   // Check the status of the method that sets the dash style for the pen.
   Status status = pen.GetLastStatus();

   if(status == Ok)
   {
      // The call to SetDashStyle was successful.
   }
   else
   {
      // There was a problem with the call to SetDashStyle.
   }
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a>
 

 
