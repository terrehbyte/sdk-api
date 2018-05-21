---
UID: NL:gdipluspath.GraphicsPath
title: GraphicsPath
author: windows-driver-content
description: A GraphicsPath object stores a sequence of lines, curves, and shapes.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPath_Class.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspath.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GraphicsPath, GraphicsPath class [GDI+], GraphicsPath class [GDI+],described, _gdiplus_CLASS_GraphicsPath_Class, gdiplus._gdiplus_CLASS_GraphicsPath_Class, gdipluspath/GraphicsPath
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: gdipluspath.h
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
req.typenames: WmfPlaceableFileHeader
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	gdipluspath.h
api_name:
-	GraphicsPath
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# GraphicsPath class


## -description


A <a href="https://msdn.microsoft.com/933dd879-480c-4b8a-965a-1656382d849a">GraphicsPath</a> object stores a sequence of lines, curves, and shapes. You can draw the entire sequence by calling the 
			<b>DrawPath</b> method of a 
			<a href="https://msdn.microsoft.com/library/windows/hardware/mt131452">Graphics</a> object. You can partition the sequence of lines, curves, and shapes into figures, and with the help of a 
			<a href="https://msdn.microsoft.com/f534b1b2-1fe3-4f30-8a7f-30d44f11d297">GraphicsPathIterator</a> object, you can draw selected figures. You can also place markers in the sequence, so that you can draw selected portions of the path.


## -remarks



A path consists of one or more figures. As you add lines and curves to a path, those lines and curves become part of a figure. You can start a new figure by calling the <a href="https://msdn.microsoft.com/3c503ff5-6f20-45bd-b61e-13dd0f3efca5">GraphicsPath::StartFigure</a> method. When you draw a path, the lines and curves within an individual figure are connected by straight lines; the ending point of one line or curve is connected to the starting point of the next line or curve. No connecting line is drawn between the end of one figure and the start of the next figure.

A figure can be open or closed. You can close a figure by calling the <a href="https://msdn.microsoft.com/8f828820-7dd6-4dd0-959c-4dcfb1ca6ac7">GraphicsPath::CloseFigure</a> method. After you call <b>GraphicsPath::CloseFigure</b>, the next line, curve, or shape that you add to the path is part of the next figure. When you draw a path, the ending point of each closed figure is automatically connected to the starting point of that figure.

Some shapes (for example, rectangles and ellipses) are intrinsically closed. When you add an intrinsically closed shape to a path, that shape is in a figure by itself, and that figure is considered closed even if you don't call <a href="https://msdn.microsoft.com/8f828820-7dd6-4dd0-959c-4dcfb1ca6ac7">GraphicsPath::CloseFigure</a>. The following methods add intrinsically closed figures to a path: 

<ul>
<li>
<a href="https://msdn.microsoft.com/5a633a04-1de4-43f5-a898-d30245567e5d">AddClosedCurve Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/39074cd8-267d-485a-8175-d0a25dcf9097">AddEllipse Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/8327b2cc-855e-419e-82c1-2a424aef2838">AddPie Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/c768a38e-0b64-4254-b844-ade567eaea8f">AddPolygon Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/b86c87c0-7d6b-4e9d-b276-a98ac9a33772">AddRectangle Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/467d4a61-8430-403c-90ed-f8c224ce3b61">AddRectangles Methods</a>
</li>
<li>
<a href="https://msdn.microsoft.com/048d67c9-1f57-4b05-b262-7d04ede69267">AddString Methods</a>
</li>
</ul>

