---
UID: NL:gdiplusimageattributes.ImageAttributes
title: ImageAttributes
author: windows-driver-content
description: An ImageAttributes object contains information about how bitmap and metafile colors are manipulated during rendering.
old-location: gdiplus\_gdiplus_CLASS_ImageAttributes_Class.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\imageattributes.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: ImageAttributes, ImageAttributes class [GDI+], ImageAttributes class [GDI+],described, _gdiplus_CLASS_ImageAttributes_Class, gdiplus._gdiplus_CLASS_ImageAttributes_Class, gdiplusimageattributes/ImageAttributes
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: gdiplusimageattributes.h
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
-	gdiplusimageattributes.h
api_name:
-	ImageAttributes
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# ImageAttributes class


## -description


An <a href="https://msdn.microsoft.com/5f3a75ad-6b86-4362-85a5-5745aec80d2b">ImageAttributes</a> object contains information about how bitmap and metafile colors are manipulated during rendering. An <b>ImageAttributes</b> object maintains several color-adjustment settings, including color-adjustment matrices, grayscale-adjustment matrices, gamma-correction values, color-map tables, and color-threshold values.


## -remarks



The colors in an image can be manipulated during rendering. They can be corrected, darkened, lightened, removed, and so on. To apply such manipulations, initialize an <a href="https://msdn.microsoft.com/5f3a75ad-6b86-4362-85a5-5745aec80d2b">ImageAttributes</a> object and pass the address of that <b>ImageAttributes</b> object (along with the address of an 
				<a href="https://msdn.microsoft.com/4962e901-cc4f-4225-8d24-731225e149e6">Image</a> object) to the 
				<a href="https://msdn.microsoft.com/8eaa8e63-a46c-4453-88a6-838785a55b9f">Graphics::DrawImage</a> method. 


