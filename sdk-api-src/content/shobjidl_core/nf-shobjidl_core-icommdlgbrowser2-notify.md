---
UID: NF:shobjidl_core.ICommDlgBrowser2.Notify
title: ICommDlgBrowser2::Notify
author: windows-driver-content
description: Called by a Shell view to notify the common dialog box hosting it that an event has occurred.
old-location: shell\ICommDlgBrowser2_Notify.htm
old-project: shell
ms.assetid: 486c306d-90ea-4ea4-afe1-2c3f5015ccf7
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: CDB2N_CONTEXTMENU_DONE, CDB2N_CONTEXTMENU_START, ICommDlgBrowser2 interface [Windows Shell],Notify method, ICommDlgBrowser2.Notify, ICommDlgBrowser2::Notify, Notify, Notify method [Windows Shell], Notify method [Windows Shell],ICommDlgBrowser2 interface, _win32_ICommDlgBrowser2_Notify, shell.ICommDlgBrowser2_Notify, shobjidl_core/ICommDlgBrowser2::Notify
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional, Windows XP [desktop apps only]
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
-	Shell32.dll
api_name:
-	ICommDlgBrowser2.Notify
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 5.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# ICommDlgBrowser2::Notify


## -description


Called by a Shell view to notify the common dialog box hosting it that an event has occurred.


## -parameters




### -param ppshv




### -param dwNotifyType

Type: <b>DWORD</b>

A flag that can can take one of the following two values.



#### CDB2N_CONTEXTMENU_START

Indicates that the shortcut menu is about to be displayed.



#### CDB2N_CONTEXTMENU_DONE

Indicates that the shortcut menu is no longer displayed.


#### - pshv

Type: <b><a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a>*</b>

A pointer to the <a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a> interface of the hosted view.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/07a416a2-340d-4308-a6f3-cf6f19f3c906">ICommDlgBrowser2</a>
 

 
