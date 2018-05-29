---
UID: NF:inked.IInkEdit.put_SelAlignment
title: IInkEdit::put_SelAlignment
author: windows-sdk-content
description: Gets or sets a value that controls the alignment of the paragraphs in an InkEdit control.
old-location: tablet\inkedit_selalignment.htm
old-project: tablet
ms.assetid: 62755220-b8e4-4f26-b5f4-8a1b4b7adc01
ms.author: windowssdkdev
ms.date: 05/24/2018
ms.keywords: 0, 1, 2, IInkEdit interface [Tablet PC],SelAlignment property, IInkEdit.SelAlignment, IInkEdit.put_SelAlignment, IInkEdit::SelAlignment, IInkEdit::get_SelAlignment, IInkEdit::put_SelAlignment, InkEdit.get_SelAlignment, InkEdit.put_SelAlignment, NULL, SelAlignment property [Tablet PC], SelAlignment property [Tablet PC],IInkEdit interface, get_SelAlignment, inked/IInkEdit::SelAlignment, inked/IInkEdit::get_SelAlignment, inked/IInkEdit::put_SelAlignment, put_SelAlignment, tablet.inkedit_selalignment
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
-	IInkEdit.SelAlignment
-	IInkEdit.get_SelAlignment
-	IInkEdit.put_SelAlignment
-	InkEdit.get_SelAlignment
-	InkEdit.put_SelAlignment
product: Windows
targetos: Windows
req.lib: InkEd.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IInkEdit::put_SelAlignment


## -description


Gets or sets a value that controls the alignment of the paragraphs in an <a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a> control.

This property is read/write.


## -parameters


## -remarks



The <b>SelAlignment</b> property determines paragraph alignment for all paragraphs that have text in the current selection or for the paragraph containing the insertion point if no text is selected.

If a selection spans multiple paragraphs with different alignment styles, the <b>SelAlignment</b> property will be null.




## -see-also




<a href="tablet.iinkedit_">IInkEdit</a>



<a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a>
 

 
