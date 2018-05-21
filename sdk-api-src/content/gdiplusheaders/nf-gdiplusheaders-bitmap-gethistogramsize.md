---
UID: NF:gdiplusheaders.Bitmap.GetHistogramSize
title: Bitmap::GetHistogramSize
author: windows-driver-content
description: The Bitmap::GetHistogramSize returns the number of elements (in an array of UINTs) that you must allocate before you call the Bitmap::GetHistogram method of a Bitmap object.
old-location: gdiplus\_gdiplus_CLASS_Bitmap_GetHistogramSize_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\bitmapclass\bitmapgethistogrammethods\gethistogramsize.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Bitmap class [GDI+],GetHistogramSize method, Bitmap.GetHistogramSize, Bitmap::GetHistogramSize, GetHistogramSize, GetHistogramSize method [GDI+], GetHistogramSize method [GDI+],Bitmap class, _gdiplus_CLASS_Bitmap_GetHistogramSize_, gdiplus._gdiplus_CLASS_Bitmap_GetHistogramSize_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusheaders.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
-	Bitmap.GetHistogramSize
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.1
---

# Bitmap::GetHistogramSize


## -description


The <b>Bitmap::GetHistogramSize</b> returns the number of elements (in an array of <b>UINT</b>s) that you must allocate before you call the <a href="https://msdn.microsoft.com/c7dcc384-54b1-457a-86cd-e27b232a9152">Bitmap::GetHistogram</a> method of a <a href="https://msdn.microsoft.com/library/windows/hardware/ff545216">Bitmap</a> object.


## -parameters




### -param format [in]

Type: <b><a href="https://msdn.microsoft.com/1769ec16-e915-4a87-83d4-0989a4d79e85">HistogramFormat</a></b>

Element of the <a href="https://msdn.microsoft.com/1769ec16-e915-4a87-83d4-0989a4d79e85">HistogramFormat</a> enumeration that specifies the pixel format of the bitmap.


### -param NumberOfEntries [out]

Type: <b>UINT*</b>

Pointer to a <b>UINT</b> that receives the number of entries.


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff545216">Bitmap</a>
 

 
