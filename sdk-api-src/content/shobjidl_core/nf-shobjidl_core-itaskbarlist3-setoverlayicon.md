---
UID: NF:shobjidl_core.ITaskbarList3.SetOverlayIcon
title: ITaskbarList3::SetOverlayIcon
author: windows-driver-content
description: Applies an overlay to a taskbar button to indicate application status or a notification to the user.
old-location: shell\ITaskbarList3_SetOverlayIcon.htm
old-project: shell
ms.assetid: 77857109-64b6-428e-b2b1-ee757784532a
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ITaskbarList3 interface [Windows Shell],SetOverlayIcon method, ITaskbarList3.SetOverlayIcon, ITaskbarList3::SetOverlayIcon, SetOverlayIcon, SetOverlayIcon method [Windows Shell], SetOverlayIcon method [Windows Shell],ITaskbarList3 interface, _shell_ITaskbarList3_SetOverlayIcon, shell.ITaskbarList3_SetOverlayIcon, shobjidl_core/ITaskbarList3::SetOverlayIcon
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
-	ITaskbarList3.SetOverlayIcon
product: Windows
targetos: Windows
req.lib: Explorerframe.lib
req.dll: Explorerframe.dll
req.irql: 
req.product: Outlook Express 6.0
---

# ITaskbarList3::SetOverlayIcon


## -description


Applies an overlay to a taskbar button to indicate application status or a notification to the user.


## -parameters




### -param hwnd [in]

Type: <b>HWND</b>

The handle of the window whose associated taskbar button receives the overlay. This handle must belong to a calling process associated with the button's application and must be a valid <b>HWND</b> or the call is ignored.


### -param hIcon [in]

Type: <b>HICON</b>

The handle of an icon to use as the overlay. This should be a small icon, measuring 16x16 pixels at 96 dpi. If an overlay icon is already applied to the taskbar button, that existing overlay is replaced.



This value can be <b>NULL</b>. How a <b>NULL</b> value is handled depends on whether the taskbar button represents a single window or a group of windows.
                        
                        <ul>
<li>If the taskbar button represents a single window, the overlay icon is removed from the display.</li>
<li>If the taskbar button represents a group of windows and a previous overlay is still available (received earlier than the current overlay, but not yet freed by a <b>NULL</b> value), then that previous overlay is displayed in place of the current overlay.</li>
</ul>


It is the responsibility of the calling application to free <i>hIcon</i> when it is no longer needed. This can generally be done after you call <b>SetOverlayIcon</b> because the taskbar makes and uses its own copy of the icon.


### -param pszDescription [in]

Type: <b>LPCWSTR</b>

A pointer to a string that provides an alt text version of the information conveyed by the overlay, for accessibility purposes.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



In versions of Windows earlier than Windows 7, applications often used icons in the notification area of the taskbar to display application status and notifications to the user. The Windows 7 taskbar allows an application to provide that same sort of user feedback through its taskbar button, centralizing more of the application information in one place. These overlays are similar to existing overlays used for shortcut icons or security notifications, displayed at the lower-right corner of the button.

The following illustration shows an overlay (the small, green square that indicates the user status as "Available") applied to the far-right taskbar button.

<img alt="Screen shot of the Windows Messenger taskbar button with an overlay to indicate an Available status" src="images/Taskbar/TaskbarOverlay.png"/>
Icon overlays serve as a contextual notification of status, and are intended to negate the need for a separate notification area status icon to communicate that information to the user. The application designer must decide during the development cycle which method—icon overlay or notification area status icon—best serves that application. Overlay icons are intended to supply important, long-standing status or notifications such as network status, messenger status, or new mail. They should not be frequently changed, nor should they be animated.

To display an overlay icon, the taskbar must be in the default large icon mode. If the taskbar is configured through <b>Taskbar and Start Menu Properties</b> to show small icons, overlays cannot be applied and calls to this method are ignored.

Because a single overlay is applied to the taskbar button instead of to the individual window thumbnails, this is a per-group feature rather than per-window. Requests for overlay icons can be received from individual windows in a taskbar group, but they do not queue. The last overlay received is the overlay shown. If the last overlay received is removed, the overlay that it replaced is restored so long as it is still active. As an example, windows 1, 2, and 3 set, in order, overlays A, B, and C. Because overlay C was received last, it is shown on the taskbar button. Window 2 calls <b>SetOverlayIcon</b> with a <b>NULL</b> value to remove overlay B. Window 3 then does the same to remove overlay C. Because window 1's overlay A is still active, that overlay is then displayed on the taskbar button.

If Windows Explorer shuts down unexpectedly, overlays are not restored when Windows Explorer is restored. The application should wait to receive the <b>TaskbarButtonCreated</b> message that indicates that Windows Explorer has restarted and the taskbar button has been re-created, and then call <b>SetOverlayIcon</b> again to reapply the overlay.




## -see-also




<a href="https://msdn.microsoft.com/c63f5fe8-4a8f-4ca8-bd6a-7733110bbb38">ITaskbarList</a>



<a href="https://msdn.microsoft.com/8af23586-349f-4d21-98cb-0aaa27a586ff">ITaskbarList2</a>



<a href="https://msdn.microsoft.com/a5eb4e5a-df17-4aca-96fb-d8475e266b92">ITaskbarList3</a>



<a href="https://msdn.microsoft.com/cbf2b07d-d67c-4755-888c-d40692d13cae">Taskbar Extensions</a>
 

 
