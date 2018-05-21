---
UID: NF:gdipluspath.GraphicsPath.GetLastPoint
title: GraphicsPath::GetLastPoint
author: windows-driver-content
description: The GraphicsPath::GetLastPoint method gets the ending point of the last figure in this path.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPath_GetLastPoint_lastPoint_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathclass\graphicspathmethods\getlastpoint.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetLastPoint, GetLastPoint method [GDI+], GetLastPoint method [GDI+],GraphicsPath class, GraphicsPath class [GDI+],GetLastPoint method, GraphicsPath.GetLastPoint, GraphicsPath::GetLastPoint, _gdiplus_CLASS_GraphicsPath_GetLastPoint_lastPoint_, gdiplus._gdiplus_CLASS_GraphicsPath_GetLastPoint_lastPoint_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspath.h
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
-	GraphicsPath.GetLastPoint
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# GraphicsPath::GetLastPoint


## -description


The <b>GraphicsPath::GetLastPoint</b> method gets the ending point of the last figure in this path.


## -parameters




### -param lastPoint [out]

Type: <b><a href="https://msdn.microsoft.com/2d357844-19a8-4ada-ba1e-685fea2e65ce">PointF</a>*</b>

Pointer to a <a href="https://msdn.microsoft.com/2d357844-19a8-4ada-ba1e-685fea2e65ce">PointF</a> object that receives the last point. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/39055c59-6d88-4b46-bc4c-cf2a4a927d29">AddLines Methods</a>



<a href="https://msdn.microsoft.com/816a5845-ca03-46c6-bdda-e6a7d02ff614">Clipping with a Region</a>



<a href="https://msdn.microsoft.com/dbfe8cea-bd9e-43ad-85c8-37cce3ef97a4">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/f6a8085c-3d6a-494f-a1ee-5fa96efb1aae">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/88fea2ec-7b53-44bb-841d-486c5c879c68">Paths</a>



<a href="https://msdn.microsoft.com/2d357844-19a8-4ada-ba1e-685fea2e65ce">PointF</a>
 

 
