---
UID: NF:gdiplusbrush.SolidBrush.SetColor
title: SolidBrush::SetColor
author: windows-driver-content
description: The SolidBrush::SetColor method sets the color of this solid brush.
old-location: gdiplus\_gdiplus_CLASS_SolidBrush_SetColor_color_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\solidbrushclass\solidbrushmethods\setcolor_9color.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: SetColor, SetColor method [GDI+], SetColor method [GDI+],SolidBrush class, SolidBrush class [GDI+],SetColor method, SolidBrush.SetColor, SolidBrush::SetColor, _gdiplus_CLASS_SolidBrush_SetColor_color_, gdiplus._gdiplus_CLASS_SolidBrush_SetColor_color_
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
-	SolidBrush.SetColor
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# SolidBrush::SetColor


## -description


The <b>SolidBrush::SetColor</b> method sets the color of this solid brush.


## -parameters




### -param color [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a></b>

Reference to a <a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a> object that specifies the color to be set in this solid brush. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/cedef138-5047-4a72-8b89-5a95062a351c">Filling a Shape with a Solid Color</a>



<a href="https://msdn.microsoft.com/8d5c8780-f03c-40b2-b237-e40121e3d6f6">SolidBrush</a>



<a href="https://msdn.microsoft.com/64bc1cb5-74a9-4789-a159-89fc35a16910">SolidBrush::GetColor</a>
 

 
