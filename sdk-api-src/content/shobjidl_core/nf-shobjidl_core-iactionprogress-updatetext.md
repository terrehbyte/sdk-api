---
UID: NF:shobjidl_core.IActionProgress.UpdateText
title: IActionProgress::UpdateText
author: windows-driver-content
description: Called if descriptive text associated with the action will be changed.
old-location: shell\IActionProgress_UpdateText.htm
old-project: shell
ms.assetid: dfb8a996-89df-4975-ac13-d871598a2787
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IActionProgress interface [Windows Shell],UpdateText method, IActionProgress.UpdateText, IActionProgress::UpdateText, UpdateText, UpdateText method [Windows Shell], UpdateText method [Windows Shell],IActionProgress interface, shell.IActionProgress_UpdateText, shell_IActionProgress_UpdateText, shobjidl_core/IActionProgress::UpdateText
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
-	Shobjidl.idl
api_name:
-	IActionProgress.UpdateText
product: Windows
targetos: Windows
req.lib: 
req.dll: Shobjidl.idl
req.irql: 
req.product: Outlook Express 6.0
---

# IActionProgress::UpdateText


## -description


Called if descriptive text associated with the action will be changed.


## -parameters




### -param sptext [in]

Type: <b><a href="https://msdn.microsoft.com/3d33cb3a-5949-446c-97ec-7ac4f4b1f675">SPTEXT</a></b>

A value that specifies the type of text displayed. See <a href="https://msdn.microsoft.com/3d33cb3a-5949-446c-97ec-7ac4f4b1f675">SPTEXT</a> for acceptable values.


### -param pszText [in]

Type: <b>LPCWSTR</b>

A pointer to a wide character string to display.


### -param fMayCompact [in]

Type: <b>BOOL</b>

A value that specifies whether to allow a text string to be compacted to fit the available space on screen.


## -returns



Type: <b>HRESULT</b>

Return S_OK if successful, or an error value otherwise.




## -remarks




		The class implementing this method must interpret the value of <i>sptext</i> and <i>fMayCompact</i> in the context of the action being performed and the UI that shows the progress to the user. The value of <i>sptext</i> can be used to differentiate between lines of changeable text. Often, the value of <i>fMayCompact</i> refers to whether the text string can be truncated with an ellipsis (...) in order to conserve screen space.
		




## -see-also




<a href="https://msdn.microsoft.com/e742e381-0fd2-482a-81a0-7b43d11b073b">IActionProgress</a>



<a href="https://msdn.microsoft.com/3d33cb3a-5949-446c-97ec-7ac4f4b1f675">SPTEXT</a>
 

 
