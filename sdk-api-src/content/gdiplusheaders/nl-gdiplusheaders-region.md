---
UID: NL:gdiplusheaders.Region
title: Region
author: windows-driver-content
description: The Region class describes an area of the display surface.
old-location: gdiplus\_gdiplus_CLASS_Region_Class.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\region.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Region, Region class [GDI+], Region class [GDI+],described, _gdiplus_CLASS_Region_Class, gdiplus._gdiplus_CLASS_Region_Class, gdiplusheaders/Region
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: gdiplusheaders.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
-	gdiplusheaders.h
api_name:
-	Region
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.0
---

# Region class


## -description


The <b>Region</b> class describes an area of the display surface. The area can be any shape. In other words, the boundary of the area can be a combination of curved and straight lines. Regions can also be created from the interiors of rectangles, paths, or a combination of these. Regions are used in clipping and hit-testing operations.


## -remarks



A GDI+ region is stored in world coordinates whereas a GDI region is stored in device coordinates. Therefore, a GDI+ region is scalable and a GDI region is not. For more information, see the <b>Scalable Regions</b> section in <a href="https://msdn.microsoft.com/0257a23c-560e-472e-863a-6ab5881dc156">New Features</a>.

An application can use regions to clip the output of drawing operations. The Window Manager uses regions to define the drawing area of windows. These regions are called clipping regions. An application can also use regions in hit-testing operations, such as checking whether a point is in a region or whether a rectangle intersects a region. For more information, see <a href="https://msdn.microsoft.com/library/windows/hardware/dn915768">Regions</a>, <a href="https://msdn.microsoft.com/58cc052d-31af-4410-81b9-defbad08a1dc">Clipping</a>, and <a href="https://msdn.microsoft.com/29a779c8-a2a4-42d8-9084-bad50ef82522">Using Regions</a>.


