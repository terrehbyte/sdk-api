---
UID: NF:gdipluspath.GraphicsPathIterator.NextPathType
title: GraphicsPathIterator::NextPathType
author: windows-driver-content
description: The GraphicsPathIterator::NextPathType method gets the starting index and the ending index of the next group of data points that all have the same type.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPathIterator_NextPathType_pathType_startIndex_endIndex_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathiteratorclass\graphicspathiteratormethods\nextpathtype.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GraphicsPathIterator class [GDI+],NextPathType method, GraphicsPathIterator.NextPathType, GraphicsPathIterator::NextPathType, NextPathType, NextPathType method [GDI+], NextPathType method [GDI+],GraphicsPathIterator class, _gdiplus_CLASS_GraphicsPathIterator_NextPathType_pathType_startIndex_endIndex_, gdiplus._gdiplus_CLASS_GraphicsPathIterator_NextPathType_pathType_startIndex_endIndex_
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
-	GraphicsPathIterator.NextPathType
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# GraphicsPathIterator::NextPathType


## -description


The <b>GraphicsPathIterator::NextPathType</b> method gets the starting index and the ending index of the next group of data points that all have the same type.


## -parameters




### -param pathType [out]

Type: <b>BYTE*</b>

Pointer to a <b>BYTE</b> that receives the point type shared by all points in the group. Possible values are PathPointTypeLine and PathPointTypeBezier, which are elements of the <a href="https://msdn.microsoft.com/daad4301-f338-4cce-bb31-ddcf09c0c59c">PathPointType</a> enumeration. 


### -param startIndex [out]

Type: <b>INT*</b>

Pointer to an <b>INT</b> that receives the starting index of the group of points. 


### -param endIndex [out]

Type: <b>INT*</b>

Pointer to an <b>INT</b> that receives the ending index of the group of points. 


## -returns



Type: <strong>Type: <b>INT</b>
</strong>

This method returns the number of data points in the group. If there are no more groups in the path, this method returns 0.




## -remarks



A path has an array of data points that define its lines and curves. All curves in the path are represented as Bézier splines, so a given point in the array has one of two types: PathPointTypeLine or PathPointTypeBezier.

The first time you call the <a href="https://msdn.microsoft.com/e7ad0477-10f6-43e0-9788-47373a40e7cd">GraphicsPathIterator::NextSubpath</a> method of an iterator, it gets the starting and ending indices of the first group of points that all have the same type. The second time, it gets the second group, and so on. Each time you call <b>GraphicsPathIterator::NextSubpath</b>, it returns the number of data points in the obtained group. When there are no groups remaining, it returns 0.




## -see-also




<a href="https://msdn.microsoft.com/dbfe8cea-bd9e-43ad-85c8-37cce3ef97a4">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/f534b1b2-1fe3-4f30-8a7f-30d44f11d297">GraphicsPathIterator</a>



<a href="https://msdn.microsoft.com/6b58521e-3093-45c7-93b4-ca658b67601f">GraphicsPathIterator::CopyData</a>



<a href="https://msdn.microsoft.com/6eb9e19c-df28-4cf9-a434-c27478ba1fa5">GraphicsPathIterator::NextMarker Methods</a>



<a href="https://msdn.microsoft.com/91137029-182d-4dc5-89a3-f3835f55d327">GraphicsPathIterator::NextSubpath Methods</a>



<a href="https://msdn.microsoft.com/88fea2ec-7b53-44bb-841d-486c5c879c68">Paths</a>
 

 
