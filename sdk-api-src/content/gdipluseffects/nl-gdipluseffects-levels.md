---
UID: NL:gdipluseffects.Levels
title: Levels
author: windows-driver-content
description: The Levels class encompasses three bitmap adjustments:\_highlight, midtone, and shadow.
old-location: gdiplus\_gdiplus_CLASS_Levels_Class.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\levels.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Levels, Levels class [GDI+], Levels class [GDI+],described, _gdiplus_CLASS_Levels_Class, gdiplus._gdiplus_CLASS_Levels_Class, gdipluseffects/Levels
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: gdipluseffects.h
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
-	gdipluseffects.h
api_name:
-	Levels
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.1
---

# Levels class


## -description


The <b>Levels</b> class encompasses three bitmap adjustments: highlight, midtone, and shadow. You can apply one or more of those adjustments to a bitmap by passing the address of a <b>Levels</b> object to the <a href="https://msdn.microsoft.com/cb85a7ac-5af0-45c7-8035-d7bc2827af6a">Graphics::DrawImage</a> method or to the <a href="https://msdn.microsoft.com/6b3d0a2f-acff-47a7-bc9f-6e9d659f683c">Bitmap::ApplyEffect</a> method. To specify the intensities of the adjustments, pass the address of a <a href="https://msdn.microsoft.com/84f6009b-ac6c-42e5-b151-9189e09c053d">LevelsParams</a> structure to the <a href="https://msdn.microsoft.com/928f88d3-1fc0-49a5-b286-794c157d10aa">Levels::SetParameters</a> method of a <b>Levels</b> object.
