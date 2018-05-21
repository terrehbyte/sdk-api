---
UID: NF:shobjidl_core.IInputObject.UIActivateIO
title: IInputObject::UIActivateIO
author: windows-driver-content
description: UI-activates or deactivates the object.
old-location: shell\IInputObject_UIActivateIO.htm
old-project: shell
ms.assetid: a725863e-4814-4aa7-99c6-7e7141db214d
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IInputObject interface [Windows Shell],UIActivateIO method, IInputObject.UIActivateIO, IInputObject::UIActivateIO, UIActivateIO, UIActivateIO method [Windows Shell], UIActivateIO method [Windows Shell],IInputObject interface, _win32_IInputObject_UIActivateIO, shell.IInputObject_UIActivateIO, shobjidl_core/IInputObject::UIActivateIO
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
-	Shell32.dll
api_name:
-	IInputObject.UIActivateIO
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.71 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IInputObject::UIActivateIO


## -description


UI-activates or deactivates the object.


## -parameters




### -param fActivate [in]

Type: <b>BOOL</b>

Indicates if the object is being activated or deactivated. If this value is nonzero, the object is being activated. If this value is zero, the object is being deactivated.


### -param pMsg [in]

Type: <b><a href="https://msdn.microsoft.com/fee176ba-ad07-4145-ab4d-1b8c335fd100">MSG</a>*</b>


          A pointer to an <a href="https://msdn.microsoft.com/fee176ba-ad07-4145-ab4d-1b8c335fd100">MSG</a> structure that contains the message that caused the activation change. This value may be <b>NULL</b>.
        


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


