---
UID: NF:gdiplusbrush.LinearGradientBrush.SetGammaCorrection
title: LinearGradientBrush::SetGammaCorrection
author: windows-driver-content
description: The LinearGradientBrush::SetGammaCorrection method specifies whether gamma correction is enabled for this linear gradient brush.
old-location: gdiplus\_gdiplus_CLASS_LinearGradientBrush_SetGammaCorrection_useGammaCorrection_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\lineargradientbrushclass\lineargradientbrushmethods\setgammacorrection.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: LinearGradientBrush class [GDI+],SetGammaCorrection method, LinearGradientBrush.SetGammaCorrection, LinearGradientBrush::SetGammaCorrection, SetGammaCorrection, SetGammaCorrection method [GDI+], SetGammaCorrection method [GDI+],LinearGradientBrush class, _gdiplus_CLASS_LinearGradientBrush_SetGammaCorrection_useGammaCorrection_, gdiplus._gdiplus_CLASS_LinearGradientBrush_SetGammaCorrection_useGammaCorrection_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusbrush.h
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
req.typenames: KnownGamingPrivileges
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Gdiplus.dll
api_name:
-	LinearGradientBrush.SetGammaCorrection
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# LinearGradientBrush::SetGammaCorrection


## -description


The <b>LinearGradientBrush::SetGammaCorrection</b> method specifies whether gamma correction is enabled for this linear gradient brush.


## -parameters




### -param useGammaCorrection [in]

Type: <b>BOOL</b>

Boolean value that specifies whether gamma correction occurs during rendering. <b>TRUE</b> specifies that gamma correction is enabled, and <b>FALSE</b> specifies that gamma correction is not enabled. By default, gamma correction is disabled during construction of a 
					<a href="https://msdn.microsoft.com/43901cd3-b059-4830-9063-e8287899e18a">LinearGradientBrush</a> object. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -remarks



Gamma correction is often done to match the intensity contrast of the gradient to the ability of the human eye to perceive intensity changes. 




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/mt297756">Color</a>



<a href="https://msdn.microsoft.com/43901cd3-b059-4830-9063-e8287899e18a">LinearGradientBrush</a>



<a href="https://msdn.microsoft.com/4d233fee-8999-4a35-92c9-1d8197fb0452">LinearGradientBrush::GetGammaCorrection</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">Rect</a>
 

 
