---
UID: NF:gdiplusbrush.HatchBrush.HatchBrush~r3
title: HatchBrush::HatchBrush~r3
author: windows-driver-content
description: Creates a HatchBrush::HatchBrush object based on a hatch style, a foreground color, and a background color.
old-location: gdiplus\_gdiplus_CLASS_HatchBrush_HatchBrush_hatchStyle_foreColor_backColor_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\hatchbrushclass\hatchbrush_47hatchstyle_forecolor_backcolor.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: HatchBrush, HatchBrush class [GDI+],HatchBrush constructor, HatchBrush constructor [GDI+], HatchBrush constructor [GDI+],HatchBrush class, HatchBrush.HatchBrush, HatchBrush.HatchBrush~r3, HatchBrush::HatchBrush, HatchBrush::HatchBrush~r3, _gdiplus_CLASS_HatchBrush_HatchBrush_hatchStyle_foreColor_backColor_, gdiplus._gdiplus_CLASS_HatchBrush_HatchBrush_hatchStyle_foreColor_backColor_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusbrush.h
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
req.typenames: KnownGamingPrivileges
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Gdiplus.dll
api_name:
-	HatchBrush.HatchBrush
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# HatchBrush::HatchBrush~r3


## -description


Creates a <b>HatchBrush::HatchBrush</b> object based on a hatch style, a foreground color, and a background color.


## -parameters






#### - backColor [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a></b>

Optional. Reference to a color to use for the background. The default value is <b>Color</b>()(a <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a> object created by the default <b>Color</b> constructor). 


#### - foreColor [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a></b>

Reference to a color to use for the hatch lines. 


#### - hatchStyle [in]

Type: <b><a href="https://msdn.microsoft.com/6321a75f-99cf-4e63-b498-168d4a8bb950">HatchStyle</a></b>

Element of the <a href="https://msdn.microsoft.com/6321a75f-99cf-4e63-b498-168d4a8bb950">HatchStyle</a> enumeration that specifies the pattern of hatch lines that will be used. 


## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/6e633cb2-8b0f-4b6a-95d8-f494d5f972eb">HatchBrush</a>



<a href="https://msdn.microsoft.com/6321a75f-99cf-4e63-b498-168d4a8bb950">HatchStyle</a>



<a href="https://msdn.microsoft.com/8ccf2c4a-6f99-465f-8adf-0f7fcd002f79">Using a Brush to Fill Shapes</a>
 

 
