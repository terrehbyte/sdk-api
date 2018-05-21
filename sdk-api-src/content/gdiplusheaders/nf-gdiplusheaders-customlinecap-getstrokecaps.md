---
UID: NF:gdiplusheaders.CustomLineCap.GetStrokeCaps
title: CustomLineCap::GetStrokeCaps
author: windows-driver-content
description: The CustomLineCap::GetStrokeCaps method gets the end cap styles for both the start line cap and the end line cap. Line caps are LineCap objects that end the individual lines within a path.
old-location: gdiplus\_gdiplus_CLASS_CustomLineCap_GetStrokeCaps_startCap_endCap_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\customlinecapclass\customlinecapmethods\getstrokecaps.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: CustomLineCap class [GDI+],GetStrokeCaps method, CustomLineCap.GetStrokeCaps, CustomLineCap::GetStrokeCaps, GetStrokeCaps, GetStrokeCaps method [GDI+], GetStrokeCaps method [GDI+],CustomLineCap class, _gdiplus_CLASS_CustomLineCap_GetStrokeCaps_startCap_endCap_, gdiplus._gdiplus_CLASS_CustomLineCap_GetStrokeCaps_startCap_endCap_
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
-	CustomLineCap.GetStrokeCaps
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# CustomLineCap::GetStrokeCaps


## -description


The <b>CustomLineCap::GetStrokeCaps</b> method gets the end cap styles for both the start line cap and the end line cap. Line caps are <a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a> objects that end the individual lines within a path.


## -parameters




### -param startCap [out]

Type: <b><a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a>*</b>

Pointer to a variable that receives an element of the <a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a> enumeration that indicates the line cap used at the start of the line to be drawn. 


### -param endCap [out]

Type: <b><a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a>*</b>

Pointer to a variable that receives an element of the <a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a> enumeration that indicates the line cap used at the end of the line to be drawn. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/bab33c8b-3203-4560-9e71-c112d528e20c">CustomLineCap</a>



<a href="https://msdn.microsoft.com/e72e402b-3cb7-4fc7-9050-ce00054da352">LineCap</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a>
 

 
