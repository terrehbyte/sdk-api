---
UID: NF:shobjidl_core.ITaskbarList3.SetTabActive
title: ITaskbarList3::SetTabActive
author: windows-driver-content
description: Informs the taskbar that a tab or document window has been made the active window.
old-location: shell\ITaskbarList3_SetTabActive.htm
old-project: shell
ms.assetid: d82f11eb-bfff-4661-8e2e-520f8226809b
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ITaskbarList3 interface [Windows Shell],SetTabActive method, ITaskbarList3.SetTabActive, ITaskbarList3::SetTabActive, SetTabActive, SetTabActive method [Windows Shell], SetTabActive method [Windows Shell],ITaskbarList3 interface, _shell_ITaskbarList3_SetTabActive, shell.ITaskbarList3_SetTabActive, shobjidl_core/ITaskbarList3::SetTabActive
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
-	Explorerframe.dll
api_name:
-	ITaskbarList3.SetTabActive
product: Windows
targetos: Windows
req.lib: Explorerframe.lib
req.dll: Explorerframe.dll
req.irql: 
req.product: Outlook Express 6.0
---

# ITaskbarList3::SetTabActive


## -description


Informs the taskbar that a tab or document window has been made the active window.


## -parameters




### -param hwndTab [in]

Type: <b>HWND</b>

Handle of the active tab window. This handle must already be registered through <a href="https://msdn.microsoft.com/b0cdca51-108a-4507-bd9e-6bcd4386c36a">ITaskbarList3::RegisterTab</a>. This value can be <b>NULL</b> if no tab is active.


### -param hwndMDI [in]

Type: <b>HWND</b>

Handle of the application's main window. This value tells the taskbar which group the thumbnail is a member of. This value is required and cannot be <b>NULL</b>.


### -param dwReserved [in]

Type: <b>DWORD</b>

Reserved; set to 0.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/c63f5fe8-4a8f-4ca8-bd6a-7733110bbb38">ITaskbarList</a>



<a href="https://msdn.microsoft.com/8af23586-349f-4d21-98cb-0aaa27a586ff">ITaskbarList2</a>



<a href="https://msdn.microsoft.com/a5eb4e5a-df17-4aca-96fb-d8475e266b92">ITaskbarList3</a>



<a href="https://msdn.microsoft.com/b0cdca51-108a-4507-bd9e-6bcd4386c36a">ITaskbarList3::RegisterTab</a>



<a href="https://msdn.microsoft.com/a35342fd-448b-48cf-8400-30f4b7776bbf">ITaskbarList3::SetTabOrder</a>



<a href="https://msdn.microsoft.com/667cafde-f693-46c3-bbec-140fc7cade5d">ITaskbarList3::UnregisterTab</a>



<a href="https://msdn.microsoft.com/cbf2b07d-d67c-4755-888c-d40692d13cae">Taskbar Extensions</a>
 

 
