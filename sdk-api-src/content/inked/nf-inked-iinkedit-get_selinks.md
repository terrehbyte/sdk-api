---
UID: NF:inked.IInkEdit.get_SelInks
title: IInkEdit::get_SelInks
author: windows-sdk-content
description: Gets or sets the array of embedded InkDisp objects (if displayed as ink) in the current selection.
old-location: tablet\inkedit_selinks.htm
old-project: tablet
ms.assetid: dbdd590d-a8d8-44e9-aecc-fbbe0d24ea20
ms.author: windowssdkdev
ms.date: 05/24/2018
ms.keywords: IInkEdit interface [Tablet PC],SelInks property, IInkEdit.SelInks, IInkEdit.get_SelInks, IInkEdit::SelInks, IInkEdit::get_SelInks, IInkEdit::put_SelInks, InkEdit.get_SelInks, InkEdit.put_SelInks, SelInks property [Tablet PC], SelInks property [Tablet PC],IInkEdit interface, dbdd590d-a8d8-44e9-aecc-fbbe0d24ea20, get_SelInks, inked/IInkEdit::SelInks, inked/IInkEdit::get_SelInks, inked/IInkEdit::put_SelInks, put_SelInks, tablet.inkedit_selinks
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: inked.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: SelAlignmentConstants
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	InkEd.dll
-	InkEd.dll.dll
api_name:
-	IInkEdit.SelInks
-	IInkEdit.get_SelInks
-	IInkEdit.put_SelInks
-	InkEdit.get_SelInks
-	InkEdit.put_SelInks
product: Windows
targetos: Windows
req.lib: InkEd.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IInkEdit::get_SelInks


## -description



Gets or sets the array of embedded <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> objects (if displayed as ink) in the current selection.



This property is read/write.


## -parameters


## -remarks



Ink must be recognized before being accessed through this property. If it is not recognized first, the <b>SelInks</b> property always contains zero <a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp</a> objects. You must either call the <a href="https://msdn.microsoft.com/e22043da-6c38-49e2-9651-43211ce7f377">Recognize</a> method (if the <a href="https://msdn.microsoft.com/e1171aa3-841f-433e-88b8-e3fc63129aeb">RecognitionTimeout</a> property equals 0) or wait until the ink is automatically recognized (when the value of the <b>RecognitionTimeout</b> property is greater than 0) to access ink through this property.

The <a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a> control ignores any <a href="https://msdn.microsoft.com/10ca7ae5-28dd-42a2-98d9-852d4de5869d">InkDrawingAttributes</a> on ink set through the <b>SelInks</b> property. Instead, the InkEdit control applies alternate drawing attributes according to the attributes of nearby text.

This property is run time only.




## -see-also




<a href="tablet.iinkedit_">IInkEdit</a>



<a href="https://msdn.microsoft.com/f942d6a3-f303-49df-a128-de9760b508ef">InkDisp Class</a>



<a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a>



<a href="https://msdn.microsoft.com/e1171aa3-841f-433e-88b8-e3fc63129aeb">RecoTimeout Property</a>



<a href="https://msdn.microsoft.com/e22043da-6c38-49e2-9651-43211ce7f377">Recognize Method [InkEdit Control]</a>
 

 
