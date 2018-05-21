---
UID: NF:gdiplusgraphics.Graphics.Clear
title: Graphics::Clear
author: windows-driver-content
description: The Graphics::Clear method clears a Graphics object to a specified color.
old-location: gdiplus\_gdiplus_CLASS_Graphics_Clear_color_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\clear.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Clear, Clear method [GDI+], Clear method [GDI+],Graphics class, Graphics class [GDI+],Clear method, Graphics.Clear, Graphics::Clear, _gdiplus_CLASS_Graphics_Clear_color_, gdiplus._gdiplus_CLASS_Graphics_Clear_color_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusgraphics.h
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
-	Graphics.Clear
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Graphics::Clear


## -description


The <b>Graphics::Clear</b> method clears a 
			<a href="https://msdn.microsoft.com/library/windows/hardware/mt131452">Graphics</a>
 object to a specified color.


## -parameters




### -param color [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a></b>

Reference to the <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a> object that specifies the color to paint the background. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/9ebd7158-26bd-447e-8351-4245e1098361">DrawRectangle Methods</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt131452">Graphics</a>
 

 
