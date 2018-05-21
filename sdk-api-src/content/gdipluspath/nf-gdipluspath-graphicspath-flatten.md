---
UID: NF:gdipluspath.GraphicsPath.Flatten
title: GraphicsPath::Flatten
author: windows-driver-content
description: The GraphicsPath::Flatten method applies a transformation to this path and converts each curve in the path to a sequence of connected lines.
old-location: gdiplus\_gdiplus_CLASS_GraphicsPath_Flatten_matrix_flatness_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\graphicspathclass\graphicspathmethods\flatten.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Flatten, Flatten method [GDI+], Flatten method [GDI+],GraphicsPath class, GraphicsPath class [GDI+],Flatten method, GraphicsPath.Flatten, GraphicsPath::Flatten, _gdiplus_CLASS_GraphicsPath_Flatten_matrix_flatness_, gdiplus._gdiplus_CLASS_GraphicsPath_Flatten_matrix_flatness_
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
-	GraphicsPath.Flatten
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# GraphicsPath::Flatten


## -description


The <b>GraphicsPath::Flatten</b> method applies a transformation to this path and converts each curve in the path to a sequence of connected lines.


## -parameters




### -param matrix [in]

Type: <b>const <a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>*</b>

Optional. Pointer to a <a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a> object that specifies the transformation to be applied to the path's data points. The default value is <b>NULL</b>, which specifies that no transformation is to be applied. 


### -param flatness [in]

Type: <b>REAL</b>

Optional. Real number that specifies the maximum error between the path and its flattened approximation. Reducing the flatness increases the number of line segments in the approximation. The default value is <code>FlatnessDefault</code>, which is a constant defined in Gdiplusenums.h. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/816a5845-ca03-46c6-bdda-e6a7d02ff614">Clipping with a Region</a>



<a href="https://msdn.microsoft.com/dbfe8cea-bd9e-43ad-85c8-37cce3ef97a4">Constructing and Drawing Paths</a>



<a href="https://msdn.microsoft.com/f6a8085c-3d6a-494f-a1ee-5fa96efb1aae">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/8ce77146-dc28-4c0b-bcf0-dad4bf3d86e8">Flattening Paths</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>



<a href="https://msdn.microsoft.com/88fea2ec-7b53-44bb-841d-486c5c879c68">Paths</a>
 

 
