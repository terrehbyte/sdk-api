---
UID: NF:gdiplusheaders.Region.FromHRGN
title: Region::FromHRGN
author: windows-driver-content
description: The Region::FromHRGN method creates a Windows GDI+Region object from a Windows Graphics Device Interface (GDI)  region.
old-location: gdiplus\_gdiplus_CLASS_Region_FromHRGN_hRgn_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\fromhrgn.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: FromHRGN, FromHRGN method [GDI+], FromHRGN method [GDI+],Region class, Region class [GDI+],FromHRGN method, Region.FromHRGN, Region::FromHRGN, _gdiplus_CLASS_Region_FromHRGN_hRgn_, gdiplus._gdiplus_CLASS_Region_FromHRGN_hRgn_
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
-	Region.FromHRGN
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Region::FromHRGN


## -description


The <b>Region::FromHRGN</b> method creates a Windows GDI+<a href="https://msdn.microsoft.com/library/windows/hardware/dn915769">Region</a> object from a Windows Graphics Device Interface (GDI)  region.


## -parameters




### -param hRgn [in]

Type: <b>HRGN</b>

Handle to an existing GDI region. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn915769">Region</a>*</b>
</strong>

This method returns a pointer to the new 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn915769">Region</a> object.


