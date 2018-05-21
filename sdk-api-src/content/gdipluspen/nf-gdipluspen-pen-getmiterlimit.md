---
UID: NF:gdipluspen.Pen.GetMiterLimit
title: Pen::GetMiterLimit
author: windows-driver-content
description: The Pen::GetMiterLimit method gets the miter length currently set for this Pen object.
old-location: gdiplus\_gdiplus_CLASS_Pen_GetMiterLimit_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\penclass\penmethods\getmiterlimit.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetMiterLimit, GetMiterLimit method [GDI+], GetMiterLimit method [GDI+],Pen class, Pen class [GDI+],GetMiterLimit method, Pen.GetMiterLimit, Pen::GetMiterLimit, _gdiplus_CLASS_Pen_GetMiterLimit_, gdiplus._gdiplus_CLASS_Pen_GetMiterLimit_
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
-	Pen.GetMiterLimit
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Pen::GetMiterLimit


## -description


The <b>Pen::GetMiterLimit</b> method gets the miter length currently set for this 
			<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object.


## -parameters






## -returns



Type: <strong>Type: <b>REAL</b>
</strong>

This method returns a real number that indicates the miter limit of this 
						<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object.




## -remarks



The miter length is the distance from the intersection of the line walls on the inside of the join to the intersection of the line walls outside of the join. The miter length can be large when the angle between two lines is small. The miter limit is the maximum allowed ratio of miter length to line width. The default value is 10.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object and gets the miter limit.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>Pen pen(Color(255,255,0,0), 4.0f);
REAL miterLimit = pen.GetMiterLimit(); </pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/4ec3e76a-2531-4869-a5b0-c595198e8345">Joining Lines</a>



<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>



<a href="https://msdn.microsoft.com/2fd2ac24-40e6-49a6-a514-1233e2075f45">Pen::SetMiterLimit</a>



<a href="https://msdn.microsoft.com/d91562ab-41e6-4bca-a320-74f490a4f88f">Pens, Lines, and Rectangles</a>
 

 
