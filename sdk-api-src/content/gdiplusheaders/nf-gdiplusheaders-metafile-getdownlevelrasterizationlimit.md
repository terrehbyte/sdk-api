---
UID: NF:gdiplusheaders.Metafile.GetDownLevelRasterizationLimit
title: Metafile::GetDownLevelRasterizationLimit
author: windows-driver-content
description: Gets the rasterization limit currently set for this metafile.
old-location: gdiplus\_gdiplus_CLASS_Metafile_GetDownLevelRasterizationLimit_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\metafileclass\metafilemethods\getdownlevelrasterizationlimit.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetDownLevelRasterizationLimit, GetDownLevelRasterizationLimit method [GDI+], GetDownLevelRasterizationLimit method [GDI+],Metafile class, Metafile class [GDI+],GetDownLevelRasterizationLimit method, Metafile.GetDownLevelRasterizationLimit, Metafile::GetDownLevelRasterizationLimit, _gdiplus_CLASS_Metafile_GetDownLevelRasterizationLimit_, gdiplus._gdiplus_CLASS_Metafile_GetDownLevelRasterizationLimit_
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
-	Metafile.GetDownLevelRasterizationLimit
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Metafile::GetDownLevelRasterizationLimit


## -description


Gets the rasterization limit currently set for this metafile. The rasterization limit is the resolution used for certain brush bitmaps that are stored in the metafile. For a detailed explanation of the rasterization limit, see <a href="https://msdn.microsoft.com/27bf1db2-e1c3-4302-8cec-61b22d97214d">Metafile::SetDownLevelRasterizationLimit</a>.


## -parameters






## -returns



Type: <strong>Type: <b>UINT</b>
</strong>

This method returns the rasterization limit in dpi.


