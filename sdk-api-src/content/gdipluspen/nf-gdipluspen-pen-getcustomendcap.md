---
UID: NF:gdipluspen.Pen.GetCustomEndCap
title: Pen::GetCustomEndCap
author: windows-driver-content
description: The Pen::GetCustomEndCap method gets the custom end cap currently set for this Pen object.
old-location: gdiplus\_gdiplus_CLASS_Pen_GetCustomEndCap_customCap_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\penclass\penmethods\getcustomendcap.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetCustomEndCap, GetCustomEndCap method [GDI+], GetCustomEndCap method [GDI+],Pen class, Pen class [GDI+],GetCustomEndCap method, Pen.GetCustomEndCap, Pen::GetCustomEndCap, _gdiplus_CLASS_Pen_GetCustomEndCap_customCap_, gdiplus._gdiplus_CLASS_Pen_GetCustomEndCap_customCap_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspen.h
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
-	Pen.GetCustomEndCap
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Pen::GetCustomEndCap


## -description


The <b>Pen::GetCustomEndCap</b> method gets the custom end cap currently set for this 
			<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object.


## -parameters




### -param customCap [out]

Type: <b><a href="https://msdn.microsoft.com/bab33c8b-3203-4560-9e71-c112d528e20c">CustomLineCap</a>*</b>

Pointer to a 
					<a href="https://msdn.microsoft.com/bab33c8b-3203-4560-9e71-c112d528e20c">CustomLineCap</a> object that receives the custom end cap of this 
					<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a> object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/0e75de3b-1006-4c8f-875c-eeb0782f24b0">Drawing a Custom Dashed Line</a>



<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>



<a href="https://msdn.microsoft.com/39a64e5c-d82b-4b0e-b851-db42996047a0">Pen::GetCustomStartCap</a>



<a href="https://msdn.microsoft.com/ba247773-7e9f-4130-a14c-42c3153e4da5">Pen::GetEndCap</a>



<a href="https://msdn.microsoft.com/4024524a-f139-4ec5-8788-b071658b8374">Pen::GetStartCap</a>



<a href="https://msdn.microsoft.com/d7be905c-92fe-4a7e-9422-f60912461dc9">Pen::SetCustomEndCap</a>



<a href="https://msdn.microsoft.com/23384bd0-94da-4c2a-9228-47cc0f0d18a7">Pen::SetCustomStartCap</a>



<a href="https://msdn.microsoft.com/d91562ab-41e6-4bca-a320-74f490a4f88f">Pens, Lines, and Rectangles</a>
 

 
