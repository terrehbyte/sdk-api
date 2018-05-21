---
UID: NL:gdiplusmatrix.Matrix
title: Matrix
author: windows-driver-content
description: A Matrix object represents a 3 &#215;3 matrix that, in turn, represents an affine transformation.
old-location: gdiplus\_gdiplus_CLASS_Matrix_Class.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\matrix.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Matrix, Matrix class [GDI+], Matrix class [GDI+],described, _gdiplus_CLASS_Matrix_Class, gdiplus._gdiplus_CLASS_Matrix_Class, gdiplusmatrix/Matrix
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: class
req.header: gdiplusmatrix.h
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
-	gdiplusmatrix.h
api_name:
-	Matrix
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Matrix class


## -description


A <b>Matrix</b> object represents a 3
			×3 matrix that, in turn, represents an affine transformation. A <b>Matrix</b> object stores only six of the 9 numbers in a 3
			×3 matrix because all 3
			×3 matrices that represent affine transformations have the same third column (0, 0, 1).
