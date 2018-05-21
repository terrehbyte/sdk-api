---
UID: NF:gdiplusbrush.LinearGradientBrush.RotateTransform
title: LinearGradientBrush::RotateTransform
author: windows-driver-content
description: The LinearGradientBrush::RotateTransform method updates this brush's current transformation matrix with the product of itself and a rotation matrix.
old-location: gdiplus\_gdiplus_CLASS_LinearGradientBrush_RotateTransform_angle_order_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\lineargradientbrushclass\lineargradientbrushmethods\rotatetransform_86angle_order.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: LinearGradientBrush class [GDI+],RotateTransform method, LinearGradientBrush.RotateTransform, LinearGradientBrush::RotateTransform, RotateTransform, RotateTransform method [GDI+], RotateTransform method [GDI+],LinearGradientBrush class, _gdiplus_CLASS_LinearGradientBrush_RotateTransform_angle_order_, gdiplus._gdiplus_CLASS_LinearGradientBrush_RotateTransform_angle_order_
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
-	LinearGradientBrush.RotateTransform
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# LinearGradientBrush::RotateTransform


## -description


The <b>LinearGradientBrush::RotateTransform</b> method updates this brush's current transformation matrix with the product of itself and a rotation matrix.


## -parameters




### -param angle [in]

Type: <b>REAL</b>

Real number that specifies the angle of rotation in degrees. 


### -param order [in]

Type: <b><a href="https://msdn.microsoft.com/df4771b2-f3c0-41c3-b2a9-4eb460162f84">MatrixOrder</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/df4771b2-f3c0-41c3-b2a9-4eb460162f84">MatrixOrder</a> enumeration that specifies the order of the multiplication. MatrixOrderPrepend specifies that the rotation matrix is on the left, and MatrixOrderAppend specifies that the rotation matrix is on the right. The default value is MatrixOrderPrepend. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a></b>
</strong>

If the method succeeds, it returns Ok, which is an element of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> enumeration.




## -remarks



A single 3
				×3 matrix can store any sequence of affine transformations. If you have several 3
				×3 matrices, each of which represents an affine transformation, the product of those matrices is a single 3
				×3 matrix that represents the entire sequence of transformations. The transformation represented by that product is called a composite transformation. For example, suppose matrix T represents a translation, and matrix R represents a rotation. If matrix M is the product TR, then matrix M represents a composite transformation: first translate, then rotate.

The order of matrix multiplication is important. In general, the matrix product RT is not the same as the matrix product TR. In the example given in the previous paragraph, the composite transformation represented by RT (first rotate, then translate) is not the same as the composite transformation represented by TR (first translate, then rotate).


#### Examples



The following example creates a linear gradient brush and uses it to fill a rectangle. Next, the code modifies the brush's transformation matrix, applying a composite transformation, and then fills a rectangle with the transformed brush.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_RotateTrans(HDC hdc)
{
   Graphics myGraphics(hdc);

   LinearGradientBrush linGrBrush(
      Rect(0, 0, 80, 40),
      Color(255, 255, 0, 0),  // red
      Color(255, 0, 0, 255),  // blue
      LinearGradientModeHorizontal);

   // Fill a large area with the linear gradient brush (no transformation).
   myGraphics.FillRectangle(&amp;linGrBrush, 0, 0, 800, 150);

   // Apply a composite transformation: first scale, then rotate.
   linGrBrush.ScaleTransform(2, 1);                    // horizontal doubling
   linGrBrush.RotateTransform(20, MatrixOrderAppend);  // 20-degree rotation

   // Fill a large area with the transformed linear gradient brush.
   myGraphics.FillRectangle(&amp;linGrBrush, 0, 200, 800, 150);  
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/e37b4c3a-b753-483a-990f-da3bcc70acf5">Filling Shapes with a Gradient Brush</a>



<a href="https://msdn.microsoft.com/43901cd3-b059-4830-9063-e8287899e18a">LinearGradientBrush</a>



<a href="https://msdn.microsoft.com/3a12c39a-a8bc-4960-a107-c8cb87af7ced">LinearGradientBrush::MultiplyTransform</a>



<a href="https://msdn.microsoft.com/ba56470e-59a4-4021-b9ce-bc13c0371007">LinearGradientBrush::ScaleTransform</a>



<a href="https://msdn.microsoft.com/ccf868a8-b5ea-40f7-b153-90b082a55374">LinearGradientBrush::TranslateTransform</a>



<a href="https://msdn.microsoft.com/92b0d9db-3d4c-47b8-87cd-60d7b4323f0a">Matrix</a>



<a href="https://msdn.microsoft.com/62215ae0-b095-42b2-911c-aa7607a8b61a">Matrix Representation of Transformations</a>



<a href="https://msdn.microsoft.com/df4771b2-f3c0-41c3-b2a9-4eb460162f84">MatrixOrder</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff569234">Rect</a>



<a href="https://msdn.microsoft.com/4acf3d70-f119-4a5b-a20d-8adea453556f">Transformations</a>
 

 
