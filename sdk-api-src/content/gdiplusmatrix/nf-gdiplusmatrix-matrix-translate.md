---
UID: NF:gdiplusmatrix.Matrix.Translate
title: Matrix::Translate
author: windows-driver-content
description: The Matrix::Translate method updates this matrix with the product of itself and a translation matrix.
old-location: gdiplus\_gdiplus_CLASS_Matrix_Translate_offsetX_offsetY_order_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\matrixclass\matrixmethods\translate.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: Matrix class [GDI+],Translate method, Matrix.Translate, Matrix::Translate, Translate, Translate method [GDI+], Translate method [GDI+],Matrix class, _gdiplus_CLASS_Matrix_Translate_offsetX_offsetY_order_, gdiplus._gdiplus_CLASS_Matrix_Translate_offsetX_offsetY_order_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusmatrix.h
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
-	Matrix.Translate
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Matrix::Translate


## -description


The <b>Matrix::Translate</b> method updates this matrix with the product of itself and a translation matrix.


## -parameters




### -param offsetX [in]

Type: <b>REAL</b>

Real number that specifies the horizontal component of the translation. 


### -param offsetY [in]

Type: <b>REAL</b>

Real number that specifies the vertical component of the translation. 


### -param order [in]

Type: <b>REAL</b>

Optional. Element of the <a href="https://msdn.microsoft.com/df4771b2-f3c0-41c3-b2a9-4eb460162f84">MatrixOrder</a> enumeration that specifies the order of the multiplication. MatrixOrderPrepend specifies that the translation matrix is on the left, and MatrixOrderAppend specifies that the translation matrix is on the right. The default value is MatrixOrderPrepend. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -see-also




<a href="https://msdn.microsoft.com/9f744c2a-f1f3-4a7e-ab0c-37aa1df01623">Global and Local Transformations</a>



<a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>



<a href="https://msdn.microsoft.com/62215ae0-b095-42b2-911c-aa7607a8b61a">Matrix Representation of Transformations</a>



<a href="https://msdn.microsoft.com/4dcf4a79-87b7-4496-907c-5a6549f1502d">Matrix::Multiply</a>



<a href="https://msdn.microsoft.com/ddbc7a4a-61aa-4daf-82ab-f1347f41f58b">Matrix::Rotate</a>



<a href="https://msdn.microsoft.com/49350cae-15f0-40ff-9655-c35432faa0ef">Matrix::RotateAt</a>



<a href="https://msdn.microsoft.com/a68cfed2-25a0-45de-83db-5f518587469a">Matrix::Scale</a>



<a href="https://msdn.microsoft.com/acf8e087-c738-4f10-a705-5c48beea6000">Matrix::Shear</a>



<a href="https://msdn.microsoft.com/df4771b2-f3c0-41c3-b2a9-4eb460162f84">MatrixOrder</a>



<a href="https://msdn.microsoft.com/4acf3d70-f119-4a5b-a20d-8adea453556f">Transformations</a>
 

 
