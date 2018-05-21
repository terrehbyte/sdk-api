---
UID: NF:gdiplusheaders.Region.Transform
title: Region::Transform
author: windows-driver-content
description: The Region::Transform method transforms this region by multiplying each of its data points by a specified matrix.
old-location: gdiplus\_gdiplus_CLASS_Region_Transform_matrix_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\transform_64matrix.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Region class [GDI+],Transform method, Region.Transform, Region::Transform, Transform, Transform method [GDI+], Transform method [GDI+],Region class, _gdiplus_CLASS_Region_Transform_matrix_, gdiplus._gdiplus_CLASS_Region_Transform_matrix_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusheaders.h
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
-	Region.Transform
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Region::Transform


## -description


The <b>Region::Transform</b> method transforms this region by multiplying each of its data points by a specified matrix.


## -parameters




### -param matrix [in]

Type: <b>const <a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>*</b>

Pointer to a matrix that specifies the transformation. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">Rect</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn915769">Region</a>



<a href="https://msdn.microsoft.com/2909bf9a-3ce0-4605-b063-e41cdc9cf317">Region::Translate Methods</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a>
 

 
