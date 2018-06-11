---
UID: NF:msinkaut.IInkDrawingAttributes.get_FitToCurve
title: IInkDrawingAttributes::get_FitToCurve
author: windows-sdk-content
description: Gets or sets the value that specifies whether Bezier smoothing is used to render ink.
old-location: tablet\inkdrawingattributes_fittocurve.htm
old-project: tablet
ms.assetid: 93b11903-84dd-4f7a-a47c-555d19fede8d
ms.author: windowssdkdev
ms.date: 06/06/2018
ms.keywords: 93b11903-84dd-4f7a-a47c-555d19fede8d, FitToCurve property [Tablet PC], FitToCurve property [Tablet PC],IInkDrawingAttributes interface, IInkDrawingAttributes interface [Tablet PC],FitToCurve property, IInkDrawingAttributes.FitToCurve, IInkDrawingAttributes.get_FitToCurve, IInkDrawingAttributes::FitToCurve, IInkDrawingAttributes::get_FitToCurve, IInkDrawingAttributes::put_FitToCurve, InkDrawingAttributes.get_FitToCurve, InkDrawingAttributes.put_FitToCurve, get_FitToCurve, msinkaut/IInkDrawingAttributes::FitToCurve, msinkaut/IInkDrawingAttributes::get_FitToCurve, msinkaut/IInkDrawingAttributes::put_FitToCurve, tablet.inkdrawingattributes_fittocurve
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: TabletPropertyMetricUnit
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - InkObj.dll
 - InkObj.dll.dll
api_name:
 - IInkDrawingAttributes.FitToCurve
 - IInkDrawingAttributes.get_FitToCurve
 - IInkDrawingAttributes.put_FitToCurve
 - InkDrawingAttributes.get_FitToCurve
 - InkDrawingAttributes.put_FitToCurve
product: Windows
targetos: Windows
req.lib: InkObj.dll
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# IInkDrawingAttributes::get_FitToCurve


## -description



Gets or sets the value that specifies whether Bezier smoothing is used to render ink.



This property is read/write.


## -parameters


## -remarks



Bezier smoothing renders ink as a series of curves instead of as lines between pen sample points. Rendering ink as a series of curves is useful for smoothing the ink, especially when the person writing the ink has unsteady writing.

If you set this property while collecting a stroke or strokes, the ink does not render as a series of curves until it is redrawn or refreshed.




## -see-also




<a href="https://msdn.microsoft.com/e39e3fc3-bcdc-4d88-8051-18ed8b183c79">GetFlattenedBezierPoints Method</a>



<a href="tablet.iinkdrawingattributes">IInkDrawingAttributes</a>



<a href="https://msdn.microsoft.com/b18464ba-feb6-4bb5-9fcf-82feff9bcce4">IInkStrokeDisp Interface</a>



<a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes Class</a>
 

 
