---
UID: NF:inked.IInkEdit.get_Font
title: IInkEdit::get_Font
author: windows-sdk-content
description: Gets or sets a Font object.
old-location: tablet\inkedit_font.htm
old-project: tablet
ms.assetid: af8234bb-7d53-45c7-9edc-fd4e6b64eed3
ms.author: windowssdkdev
ms.date: 05/24/2018
ms.keywords: Font property [Tablet PC], Font property [Tablet PC],IInkEdit interface, IInkEdit interface [Tablet PC],Font property, IInkEdit.Font, IInkEdit.get_Font, IInkEdit::Font, IInkEdit::get_Font, IInkEdit::put_Font, InkEdit.get_Font, InkEdit.put_Font, get_Font, inked/IInkEdit::Font, inked/IInkEdit::get_Font, inked/IInkEdit::put_Font, put_Font, tablet.inkedit_font
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
-	IInkEdit.Font
-	IInkEdit.get_Font
-	IInkEdit.put_Font
-	InkEdit.get_Font
-	InkEdit.put_Font
product: Windows
targetos: Windows
req.lib: InkEd.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IInkEdit::get_Font


## -description


Gets or sets a Font object.

This property is read/write.


## -parameters


## -remarks



Use the <b>Font</b> property of an <a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a> control to identify a specific Font object whose properties you want to use. For example, the following code changes the <b>Bold</b> property setting of a Font object identified by the <b>Font</b> property of an InkEdit control:

<code>myInkEditControl.Font.Bold = true;</code>




## -see-also




<a href="tablet.iinkedit_">IInkEdit</a>



<a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a>
 

 
