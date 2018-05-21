---
UID: NF:shobjidl_core.IShellFolder.GetAttributesOf
title: IShellFolder::GetAttributesOf
author: windows-driver-content
description: Gets the attributes of one or more file or folder objects contained in the object represented by IShellFolder.
old-location: shell\IShellFolder_GetAttributesOf.htm
old-project: shell
ms.assetid: 3864b386-7653-4661-880c-e96c08ff0dbb
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetAttributesOf, GetAttributesOf method [Windows Shell], GetAttributesOf method [Windows Shell],IShellFolder interface, GetAttributesOf method [Windows Shell],IShellFolder2 interface, IShellFolder interface [Windows Shell],GetAttributesOf method, IShellFolder.GetAttributesOf, IShellFolder2 interface [Windows Shell],GetAttributesOf method, IShellFolder2::GetAttributesOf, IShellFolder::GetAttributesOf, _win32_IShellFolder_GetAttributesOf, shell.IShellFolder_GetAttributesOf, shobjidl_core/IShellFolder2::GetAttributesOf, shobjidl_core/IShellFolder::GetAttributesOf
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
-	IShellFolder.GetAttributesOf
-	IShellFolder2.GetAttributesOf
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellFolder::GetAttributesOf


## -description


Gets the attributes of one or more file or folder objects contained in the object represented by <a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>.


## -parameters




### -param cidl [in]

Type: <b>UINT</b>

The number of items from which to retrieve attributes.


### -param apidl [in]

Type: <b>PCUITEMID_CHILD_ARRAY*</b>

The address of an array of pointers to <a href="https://msdn.microsoft.com/60daf071-4e93-4e1c-bc38-894f706db04f">ITEMIDLIST</a> structures, each of which uniquely identifies an item relative to the parent folder. Each <b>ITEMIDLIST</b> structure must contain exactly one <a href="https://msdn.microsoft.com/794c8425-2319-4339-881c-c5083ab05638">SHITEMID</a> structure followed by a terminating zero.


### -param rgfInOut [in, out]

Type: <b>SFGAOF*</b>

Pointer to a single <b>ULONG</b> value that, on entry, contains the bitwise <a href="https://msdn.microsoft.com/4cb85995-cdc8-4474-8c4d-c783ac91c759">SFGAO</a> attributes that the calling application is requesting. On exit, this value contains the requested attributes that are common to all of the specified items.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



To optimize this operation, do not return unspecified flags.

For a folder object, the <a href="https://msdn.microsoft.com/4cb85995-cdc8-4474-8c4d-c783ac91c759">SFGAO_BROWSABLE</a> attribute implies that the client can bind to this object as shown in a general form here.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>IShellFolder::BindToObject(..., pidl, IID_IShellFolder, &amp;psfItem);
</pre>
</td>
</tr>
</table></span></div>
The client can then create an <a href="https://msdn.microsoft.com/91438583-e4f1-456f-a130-2a45846fd725">IShellView</a> on that item through this statement.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>psfItem-&gt;CreateViewObject(..., IID_IShellView,...);
</pre>
</td>
</tr>
</table></span></div>
The <a href="https://msdn.microsoft.com/4cb85995-cdc8-4474-8c4d-c783ac91c759">SFGAO_DROPTARGET</a> attribute implies that the client can bind to an instance of <a href="https://msdn.microsoft.com/13fbe834-1ef8-4944-b2e4-9f5c413c65c8">IDropTarget</a> for this folder by calling <a href="https://msdn.microsoft.com/ec863dbf-8ec9-4952-8912-575125e6dd09">IShellFolder::GetUIObjectOf</a> as shown here.

                

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>IShellFolder::GetUIObjectOf(hwnd, 1, &amp;pidl, IID_IDropTarget, NULL, &amp;pv)
</pre>
</td>
</tr>
</table></span></div>
The SFGAO_NONENUMERATED attribute indicates an item that is not returned by the enumerator created by the <a href="https://msdn.microsoft.com/248bec8b-0bf4-47d5-adb3-31a685a2c359">IShellFolder::EnumObjects</a> method.




## -see-also




<a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>



<a href="https://msdn.microsoft.com/9b008034-3576-429e-b67c-e2222592ca46">IShellFolder2</a>
 

 
