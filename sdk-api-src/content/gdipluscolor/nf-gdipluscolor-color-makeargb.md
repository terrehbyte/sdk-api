---
UID: NF:gdipluscolor.Color.MakeARGB
title: Color::MakeARGB
author: windows-driver-content
description: The Color::MakeARGB method creates a 32-bit value that consolidates the specified alpha, red, green, and blue components.
old-location: gdiplus\_gdiplus_CLASS_Color_MakeARGB_a_r_g_b_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\colorclass\colormethods\makeargb.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Color class [GDI+],MakeARGB method, Color.MakeARGB, Color::MakeARGB, MakeARGB, MakeARGB method [GDI+], MakeARGB method [GDI+],Color class, _gdiplus_CLASS_Color_MakeARGB_a_r_g_b_, gdiplus._gdiplus_CLASS_Color_MakeARGB_a_r_g_b_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluscolor.h
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
-	Color.MakeARGB
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Color::MakeARGB


## -description


The <b>Color::MakeARGB</b> method creates a 32-bit value that consolidates the specified alpha, red, green, and blue components.


## -parameters




### -param a [in]

Type: <b>BYTE</b>

Byte that specifies the alpha component. 


### -param r [in]

Type: <b>BYTE</b>

Byte that specifies the red component. 


### -param g [in]

Type: <b>BYTE</b>

Byte that specifies the green component. 


### -param b [in]

Type: <b>BYTE</b>

Byte that specifies the blue component. 


## -returns



Type: <strong>Type: <b>static</b>
</strong>

This method returns an <b>ARGB</b> value that holds the specified alpha, red, green, and blue components.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/b333bf7d-b212-43fd-8f86-d7bf73b6a3f4">Color::GetValue</a>



<a href="https://msdn.microsoft.com/5fb15f81-8bed-4895-bec8-b687028cc5a2">Color::SetFromCOLORREF</a>
 

 
