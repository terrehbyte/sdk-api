---
UID: NF:gdiplusheaders.Image.SelectActiveFrame
title: Image::SelectActiveFrame
author: windows-driver-content
description: The Image::SelectActiveFrame method selects the frame in this Image object specified by a dimension and an index.
old-location: gdiplus\_gdiplus_CLASS_Image_SelectActiveFrame_dimensionID_frameIndex_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\imageclass\imagemethods\selectactiveframe.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Image class [GDI+],SelectActiveFrame method, Image.SelectActiveFrame, Image::SelectActiveFrame, SelectActiveFrame, SelectActiveFrame method [GDI+], SelectActiveFrame method [GDI+],Image class, _gdiplus_CLASS_Image_SelectActiveFrame_dimensionID_frameIndex_, gdiplus._gdiplus_CLASS_Image_SelectActiveFrame_dimensionID_frameIndex_
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
-	Image.SelectActiveFrame
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Image::SelectActiveFrame


## -description


The <b>Image::SelectActiveFrame</b> method selects the frame in this 
			<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a> object specified by a dimension and an index.


## -parameters




### -param dimensionID [in]

Type: <b>const GUID*</b>

Pointer to a 
					<b>GUID</b> that specifies the frame dimension. 
					<b>GUID</b>s that identify various frame dimensions are defined in Gdiplusimaging.h. 


### -param frameIndex [in]

Type: <b>UINT</b>

Integer that specifies the index of the frame within the specified frame dimension. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

<b>Remarks</b>

When you call the <b>Image::SelectActiveFrame</b> method, all changes that you made to the previously active frame are discarded. If you want to retain changes that you make to a frame, call the 
						<b>Save</b> method before you switch to a different frame.

Among all the image formats currently supported by GDI+, the only formats that support multiple-frame images are GIF and TIFF. When you call the <b>Image::SelectActiveFrame</b> method on a GIF image, you should use FrameDimensionTime. When you call the <b>Image::SelectActiveFrame</b> method on a TIFF image, you should use FrameDimensionPage.




## -see-also




<a href="https://msdn.microsoft.com/1ea22bdc-c519-466e-ad39-192910785f4b">EncoderParameter</a>



<a href="https://msdn.microsoft.com/347275b5-22d2-47ad-9754-0bd213689bf0">EncoderParameters</a>



<a href="https://msdn.microsoft.com/454d35be-ccb6-4a91-ba12-b07d55526f8e">GetImageEncoders</a>



<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a>



<a href="https://msdn.microsoft.com/ea264188-3c39-4f00-84f3-114c81a5642e">Image::Save Methods</a>



<a href="https://msdn.microsoft.com/e597f6e6-6e07-4afb-8905-26e4af961685">Image::SaveAdd Methods</a>



<a href="https://msdn.microsoft.com/f9a5b4b1-4e25-42c8-a96b-a3104841e5f3">Using Image Encoders and Decoders</a>
 

 
