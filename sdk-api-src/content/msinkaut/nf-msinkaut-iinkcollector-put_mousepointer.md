---
UID: NF:msinkaut.IInkCollector.put_MousePointer
title: IInkCollector::put_MousePointer
author: windows-driver-content
description: Gets or sets a value that indicates the type of mouse pointer that appears.
old-location: tablet\inkcollector_mousepointer.htm
old-project: tablet
ms.assetid: 8876b0ef-1a61-481b-ac37-9e4d637f8097
ms.author: windowsdriverdev
ms.date: 5/17/2018
ms.keywords: 8876b0ef-1a61-481b-ac37-9e4d637f8097, IInkCollector.put_MousePointer, IInkCollector::put_MousePointer, InkCollector class [Tablet PC],MousePointer property, InkCollector.MousePointer, InkCollector.get_MousePointer, InkCollector.put_MousePointer, MousePointer property [Tablet PC], MousePointer property [Tablet PC],InkCollector class, get_MousePointer, put_MousePointer, tablet.inkcollector_mousepointer
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: msinkaut.h
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
req.typenames: TabletPropertyMetricUnit
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	InkObj.dll
-	InkObj.dll.dll
api_name:
-	InkCollector.MousePointer
-	put_MousePointer
-	IInkCollector.put_MousePointer
-	InkCollector.get_MousePointer
-	InkCollector.put_MousePointer
product: Windows
targetos: Windows
req.lib: InkObj.dll
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# IInkCollector::put_MousePointer


## -description



Gets or sets a value that indicates the type of mouse pointer that appears.



This property is read/write.


## -parameters


## -remarks



If you set the <b>MousePointer</b> property to <a href="https://msdn.microsoft.com/74f489f2-d568-4133-96e6-de15cbfabfe7">IMP_Default</a>, the mouse cursor setting is based on the current cursor's drawing attributes. If the ink collector is disabled, the mouse cursor setting is based on the underlying windows mouse cursor <a href="https://msdn.microsoft.com/de8b2473-092d-4ff9-adbc-3ba378b035e2">DrawingAttributes</a> property. If the <b>MousePointer</b> property is set to <b>IMP_Custom</b> and the <a href="https://msdn.microsoft.com/9c7f879a-1b6c-4bd0-8dc1-82f23ace57c4">MouseIcon</a> property is <b>NULL</b>, then the ink collector no longer handles mouse cursor settings. Setting the mouse cursor to any other setting (other than the <b>MousePointer</b> property set to <b>IMP_Default</b> and the <b>MouseIcon</b> property set to <b>NULL</b>) forces the mouse cursor to use the current setting.

You can use this property when you want to indicate changes in functionality as the mouse pointer passes over controls on a form or dialog box. The <a href="https://msdn.microsoft.com/74f489f2-d568-4133-96e6-de15cbfabfe7">IMP_Hourglass</a> setting is useful for indicating that the user should wait for a process or operation to finish.




## -see-also




<a href="https://msdn.microsoft.com/189f430e-9d00-4e29-bb8c-8ac195896793">InkCollector</a>



<a href="https://msdn.microsoft.com/74f489f2-d568-4133-96e6-de15cbfabfe7">InkMousePointer Enumeration</a>



<a href="https://msdn.microsoft.com/9c7f879a-1b6c-4bd0-8dc1-82f23ace57c4">MouseIcon Property</a>
 

 
