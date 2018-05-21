---
UID: NF:shobjidl_core.IActionProgress.Begin
title: IActionProgress::Begin
author: windows-driver-content
description: Called when an action has begun that requires its progress be displayed to the user.
old-location: shell\IActionProgress_Begin.htm
old-project: shell
ms.assetid: c26dd072-6d59-4c6c-a273-682ded994612
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: Begin, Begin method [Windows Shell], Begin method [Windows Shell],IActionProgress interface, IActionProgress interface [Windows Shell],Begin method, IActionProgress.Begin, IActionProgress::Begin, shell.IActionProgress_Begin, shell_IActionProgress_Begin, shobjidl_core/IActionProgress::Begin
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
-	IActionProgress.Begin
product: Windows
targetos: Windows
req.lib: 
req.dll: Shobjidl.idl
req.irql: 
req.product: Outlook Express 6.0
---

# IActionProgress::Begin


## -description


Called when an action has begun that requires its progress be displayed to the user.


## -parameters




### -param action [in]

Type: <b><a href="https://msdn.microsoft.com/fc5a0f96-e8c2-483f-86b0-d8c870a9f77a">SPACTION</a></b>

The action being performed. See <a href="https://msdn.microsoft.com/fc5a0f96-e8c2-483f-86b0-d8c870a9f77a">SPACTION</a> for a list of acceptable values.


### -param flags [in]

Type: <b><a href="https://msdn.microsoft.com/dc5215ca-17c8-47c1-8059-f46400ff1d0f">SPBEGINF</a></b>

Optional flags that request certain UI operations be enabled or disabled. See <a href="https://msdn.microsoft.com/dc5215ca-17c8-47c1-8059-f46400ff1d0f">SPBEGINF</a> for a list of acceptable values.


## -returns



Type: <b>HRESULT</b>

Return S_OK if successful, or an error value otherwise.




## -remarks




			This method should be called when an action is beginning. The values of <i>action</i> and <i>flags</i> may be used to determine how to draw the UI that will be displayed to the user, or how to interpret or filter certain user actions associated with the action. When the action has completed, <a href="https://msdn.microsoft.com/91fa11c3-c781-4e96-9a42-4625b8b24333">IActionProgress::End</a> should be called.
			




## -see-also




<a href="https://msdn.microsoft.com/e742e381-0fd2-482a-81a0-7b43d11b073b">IActionProgress</a>



<a href="https://msdn.microsoft.com/91fa11c3-c781-4e96-9a42-4625b8b24333">IActionProgress::End</a>



<a href="https://msdn.microsoft.com/fc5a0f96-e8c2-483f-86b0-d8c870a9f77a">SPACTION</a>



<a href="https://msdn.microsoft.com/dc5215ca-17c8-47c1-8059-f46400ff1d0f">SPBEGINF</a>
 

 
