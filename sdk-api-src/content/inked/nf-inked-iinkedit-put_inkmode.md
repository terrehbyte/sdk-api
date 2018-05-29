---
UID: NF:inked.IInkEdit.put_InkMode
title: IInkEdit::put_InkMode
author: windows-sdk-content
description: Gets or sets a value that specifies whether ink collection is disabled, ink is collected, or ink and gestures are collected.
old-location: tablet\inkedit_inkmode.htm
old-project: tablet
ms.assetid: 0e395907-108b-40cf-819b-65a34e4ffc4d
ms.author: windowssdkdev
ms.date: 05/24/2018
ms.keywords: 0e395907-108b-40cf-819b-65a34e4ffc4d, Disabled, IInkEdit interface [Tablet PC],InkMode property, IInkEdit.InkMode, IInkEdit.put_InkMode, IInkEdit::InkMode, IInkEdit::get_InkMode, IInkEdit::put_InkMode, Ink, InkAndGesture, InkEdit.get_InkMode, InkEdit.put_InkMode, InkMode property [Tablet PC], InkMode property [Tablet PC],IInkEdit interface, get_InkMode, inked/IInkEdit::InkMode, inked/IInkEdit::get_InkMode, inked/IInkEdit::put_InkMode, put_InkMode, tablet.inkedit_inkmode
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
-	IInkEdit.InkMode
-	IInkEdit.get_InkMode
-	IInkEdit.put_InkMode
-	InkEdit.get_InkMode
-	InkEdit.put_InkMode
product: Windows
targetos: Windows
req.lib: InkEd.dll
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IInkEdit::put_InkMode


## -description



Gets or sets a value that specifies whether ink collection is disabled, ink is collected, or ink and gestures are collected.



This property is read/write.


## -parameters


## -remarks



The value of this property is always Disabled if it is used on a system that has Microsoft Windows XP Tablet PC Edition installed but no recognizers are present. If used on a system with Windows Vista or Windows XP Tablet PC Edition installed, the value can be set to any of the values in the <a href="https://msdn.microsoft.com/81aac302-c89a-42ca-9c90-170611a8995a">InkMode</a> enumeration type.

This property should be changed only if the <a href="https://msdn.microsoft.com/library/windows/hardware/dn265407">Status</a> property returns IES_Idle.




## -see-also




<a href="tablet.iinkedit_">IInkEdit</a>



<a href="https://msdn.microsoft.com/52761cb2-4433-4824-ba19-fe597de2faf0">InkEdit</a>



<a href="https://msdn.microsoft.com/81aac302-c89a-42ca-9c90-170611a8995a">InkMode Enumeration</a>
 

 
