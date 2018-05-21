---
UID: NF:gdiplusgraphics.Graphics.GetNearestColor
title: Graphics::GetNearestColor
author: windows-driver-content
description: The Graphics::GetNearestColor method gets the nearest color to the color that is passed in. This method works on 8-bits per pixel or lower display devices for which there is an 8-bit color palette.
old-location: gdiplus\_gdiplus_CLASS_Graphics_GetNearestColor_color_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicsclass\graphicsmethods\getnearestcolor.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetNearestColor, GetNearestColor method [GDI+], GetNearestColor method [GDI+],Graphics class, Graphics class [GDI+],GetNearestColor method, Graphics.GetNearestColor, Graphics::GetNearestColor, _gdiplus_CLASS_Graphics_GetNearestColor_color_, gdiplus._gdiplus_CLASS_Graphics_GetNearestColor_color_
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
-	Graphics.GetNearestColor
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Graphics::GetNearestColor


## -description


The <b>Graphics::GetNearestColor</b> method gets the nearest color to the color that is passed in. This method works on 8-bits per pixel or lower display devices for which there is an 8-bit color palette.


## -parameters




### -param color [in, out]

Type: <b>Color*</b>

Pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a> object that, on input, specifies the color to be tested and, on output, receives the nearest color found in the color palette. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt131452">Graphics</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a>
 

 
