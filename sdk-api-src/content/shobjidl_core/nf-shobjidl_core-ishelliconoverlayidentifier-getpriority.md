---
UID: NF:shobjidl_core.IShellIconOverlayIdentifier.GetPriority
title: IShellIconOverlayIdentifier::GetPriority
author: windows-driver-content
description: Specifies the priority of an icon overlay.
old-location: shell\IShellIconOverlayIdentifier_GetPriority.htm
old-project: shell
ms.assetid: c191bcf7-8b49-4276-9e30-2a8dcaf1fc46
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetPriority, GetPriority method [Windows Shell], GetPriority method [Windows Shell],IShellIconOverlayIdentifier interface, IShellIconOverlayIdentifier interface [Windows Shell],GetPriority method, IShellIconOverlayIdentifier.GetPriority, IShellIconOverlayIdentifier::GetPriority, _win32_IShellIconOverlayIdentifier_GetPriority, shell.IShellIconOverlayIdentifier_GetPriority, shobjidl_core/IShellIconOverlayIdentifier::GetPriority
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shlobj.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
-	Shell32.dll
api_name:
-	IShellIconOverlayIdentifier.GetPriority
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellIconOverlayIdentifier::GetPriority


## -description


Specifies the priority of an icon overlay.


## -parameters




### -param pPriority [out]

Type: <b>int*</b>

The address of a value that indicates the priority of the overlay identifier. Possible values range from zero to 100, with zero the highest priority.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if successful, or a COM error code otherwise.




## -remarks



If more than one icon overlay is available for an object, the one with highest priority is chosen. The Shell has a set of internal rules that determine priority for many cases. The value returned by <b>GetPriority</b> is used for those cases in which the Shell's internal rules do not apply. Typically, you should set the value to zero. However, the priority value is useful when you have implemented two or more icon overlay handlers that can request icon overlay icons for the same object. By setting the priority values appropriately, you can specify which of the requested icon overlays will be displayed.
      




## -see-also




<a href="https://msdn.microsoft.com/c093bc13-def7-411d-b741-50996ffad84b">IShellIconOverlayIdentifier</a>
 

 
