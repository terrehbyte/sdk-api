---
UID: NF:gdiplustypes.Size.Empty
title: Size::Empty
author: windows-driver-content
description: The Size::Empty method determines whether a Size object is empty.
old-location: gdiplus\_gdiplus_CLASS_Size_Empty_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\sizeclass\sizemethods\empty.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Empty, Empty method [GDI+], Empty method [GDI+],Size class, Size class [GDI+],Empty method, Size.Empty, Size::Empty, _gdiplus_CLASS_Size_Empty_, gdiplus._gdiplus_CLASS_Size_Empty_
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
-	Size.Empty
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Size::Empty


## -description


The <b>Size::Empty</b> method determines whether a 
			<a href="https://msdn.microsoft.com/library/windows/hardware/dn915850">Size</a> object is empty.


## -parameters






## -returns



Type: <strong>Type: <b>BOOL</b>
</strong>

If the 
						<b>Width</b> and 
						<b>Height</b> data members are both equal to zero, this method returns <b>TRUE</b>; otherwise, it returns <b>FALSE</b>.




## -remarks



A 
				<a href="https://msdn.microsoft.com/library/windows/hardware/dn915850">Size</a> object is defined as empty if the 
				<b>Width</b> and 
				<b>Height</b> data members are both equal to zero.


#### Examples



<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>Rect rect(50, 50, 100, 200);
Size size;

rect.Inflate(-50, -100);
rect.GetSize(&amp;size);

if(size.Empty())
{
   // The width and height are both 0.
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">Rect</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn915850">Size</a>



<a href="https://msdn.microsoft.com/b40ade07-f89e-44ba-9185-9aec01f1051f">SizeF</a>
 

 
