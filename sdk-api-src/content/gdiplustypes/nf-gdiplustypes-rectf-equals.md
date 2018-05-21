---
UID: NF:gdiplustypes.RectF.Equals
title: RectF::Equals
author: windows-driver-content
description: The RectF::Equals method determines whether two rectangles are the same.
old-location: gdiplus\_gdiplus_CLASS_RectF_Equals_rect_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\rectfclass\rectfmethods\equals_30rect.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Equals, Equals method [GDI+], Equals method [GDI+],RectF class, RectF class [GDI+],Equals method, RectF.Equals, RectF::Equals, _gdiplus_CLASS_RectF_Equals_rect_, gdiplus._gdiplus_CLASS_RectF_Equals_rect_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplustypes.h
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
-	RectF.Equals
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# RectF::Equals


## -description


The <b>RectF::Equals</b> method determines whether two rectangles are the same. 


## -parameters




### -param rect [in]

Type: <b>const RectF&amp;</b>

Reference to a rectangle to compare to this rectangle. 


## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the rectangles are the same, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -remarks



Two rectangles are the same if their 
				<b>X</b>, 
				<b>Y</b>, 
				<b>Width</b>, and 
				<b>Height</b> data members are the same.


#### Examples



The following example creates two 
						<a href="https://msdn.microsoft.com/6821442b-d352-48cb-a48a-839105a8c36a">RectF</a> objects, moves the second 
						<b>RectF</b> object horizontally by a specified value, and then determines whether the two 
						<b>RectF</b> objects are the same.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_Equals(HDC hdc)
{
   Graphics graphics(hdc);

   RectF rect1(50, 50, 200, 100);
   RectF rect2(20, 50, 200, 100);

   rect2.Offset(30, 0);

   if(rect2.Equals(rect1))
   {
      // The two rectangles are the same.
   }
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/d91562ab-41e6-4bca-a320-74f490a4f88f">Pens, Lines, and Rectangles</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">Rect</a>



<a href="https://msdn.microsoft.com/6821442b-d352-48cb-a48a-839105a8c36a">RectF</a>



<a href="https://msdn.microsoft.com/f2e4144f-f2f1-49db-bfdf-ffce3023b4cb">Using a Pen to Draw Lines and Rectangles</a>
 

 
