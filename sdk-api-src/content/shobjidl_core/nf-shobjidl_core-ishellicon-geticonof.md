---
UID: NF:shobjidl_core.IShellIcon.GetIconOf
title: IShellIcon::GetIconOf
author: windows-driver-content
description: Gets an icon for an object inside a specific folder.
old-location: shell\IShellIcon_GetIconOf.htm
old-project: shell
ms.assetid: 42ab02bf-7b94-447d-9a09-d1f4a47bef5d
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: 0, 1, 2, 3, 4, GIL_FORSHELL, GIL_OPENICON, GetIconOf, GetIconOf method [Windows Shell], GetIconOf method [Windows Shell],IShellIcon interface, IShellIcon interface [Windows Shell],GetIconOf method, IShellIcon.GetIconOf, IShellIcon::GetIconOf, _win32_IShellIcon_GetIconOf, shell.IShellIcon_GetIconOf, shobjidl_core/IShellIcon::GetIconOf
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
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
-	IShellIcon.GetIconOf
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellIcon::GetIconOf


## -description


Gets an icon for an object inside a specific folder.


## -parameters




### -param pidl

Type: <b>LPCITEMIDLIST</b>

The address of the <a href="https://msdn.microsoft.com/60daf071-4e93-4e1c-bc38-894f706db04f">ITEMIDLIST</a> structure that specifies the relative location of the folder.


### -param flags

Type: <b>UINT</b>

Flags specifying how the icon is to display. This parameter can be zero or one of the following values.



#### GIL_FORSHELL

The icon is to be displayed in a Shell folder.



#### GIL_OPENICON

The icon should be in the open state if both open-state and closed-state images are available. If this flag is not specified, the icon should be in the closed state. This flag is typically used for folder objects.


### -param pIconIndex






#### - lpIconIndex

Type: <b>LPINT</b>

The address of the index of the icon in the system image list. The following standard image list indexes can be returned.



#### 0

Document (blank page, not associated)



#### 1

Document (with data on the page)



#### 2

Application (file name extension must be .exe, .com, or .bat)



#### 3

Folder (plain)



#### 4

Folder (open)


## -returns



Type: <b>HRESULT</b>

Returns S_OK if <i>lpIconIndex</i> contains the correct system image list index, or S_FALSE if an icon can't be obtained for this object.




## -remarks



If you are unable to retrieve an icon for this object using <b>GetIconOf</b>, use the <a href="https://msdn.microsoft.com/ec863dbf-8ec9-4952-8912-575125e6dd09">GetUIObjectOf</a> method to retrieve an object that supports the <a href="https://msdn.microsoft.com/3ce54876-e4f8-4f9a-8e1c-ec1db691f020">Extract</a> method.

<b>IShellIcon::GetIconOf</b> fails if <a href="https://msdn.microsoft.com/0f171cf4-87b9-43a6-97f2-80ed344fe376">CoInitialize</a> is not called first.

<h3><a id="Note_to_Calling_Applications"></a><a id="note_to_calling_applications"></a><a id="NOTE_TO_CALLING_APPLICATIONS"></a>Note to Calling Applications</h3>
The index returned is from the system image list.

<h3><a id="Note_to_Implementers"></a><a id="note_to_implementers"></a><a id="NOTE_TO_IMPLEMENTERS"></a>Note to Implementers</h3>
If the icon index used is not one of the standard images listed, it is the implementer's responsibility to add the image to the system image list and then place the index into the <i>lpIconIndex</i> parameter. To prevent the system image list from growing too large, each image should only be added once.




## -see-also




<a href="https://msdn.microsoft.com/64711453-bc70-4acb-bff7-8b5534cceff5">IShellIcon</a>
 

 
