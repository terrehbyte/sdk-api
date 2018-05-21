---
UID: NF:shobjidl_core.IShellFolder.ParseDisplayName
title: IShellFolder::ParseDisplayName
author: windows-driver-content
description: Translates the display name of a file object or a folder into an item identifier list.
old-location: shell\IShellFolder_ParseDisplayName.htm
old-project: shell
ms.assetid: 099e71b0-04f2-4f82-aa00-7581bd357900
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IShellFolder interface [Windows Shell],ParseDisplayName method, IShellFolder.ParseDisplayName, IShellFolder2 interface [Windows Shell],ParseDisplayName method, IShellFolder2::ParseDisplayName, IShellFolder::ParseDisplayName, ParseDisplayName, ParseDisplayName method [Windows Shell], ParseDisplayName method [Windows Shell],IShellFolder interface, ParseDisplayName method [Windows Shell],IShellFolder2 interface, _win32_IShellFolder_ParseDisplayName, shell.IShellFolder_ParseDisplayName, shobjidl_core/IShellFolder2::ParseDisplayName, shobjidl_core/IShellFolder::ParseDisplayName
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
-	IShellFolder.ParseDisplayName
-	IShellFolder2.ParseDisplayName
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll (version 4.0 or later)
req.irql: 
req.product: Outlook Express 6.0
---

# IShellFolder::ParseDisplayName


## -description


Translates the display name of a file object or a folder into an item identifier list.


## -parameters




### -param hwnd [in]

Type: <b>HWND</b>

A window handle. The client should provide a window handle if it displays a dialog or message box. Otherwise set <i>hwnd</i> to <b>NULL</b>.


### -param pbc [in]

Type: <b><a href="https://msdn.microsoft.com/e4c8abb5-0c89-44dd-8d95-efbfcc999b46">IBindCtx</a>*</b>

Optional. A pointer to a bind context used to pass parameters as inputs and outputs to the parsing function. These passed parameters are often specific to the data source and are documented by the data source owners. For example, the file system data source accepts the name being parsed (as a <a href="https://msdn.microsoft.com/eb700d84-0ba5-4af8-a619-2d2544560dbc">WIN32_FIND_DATA</a> structure), using the <a href="https://msdn.microsoft.com/d89a0ee1-9a4b-48a4-8965-0d92f09743a6">STR_FILE_SYS_BIND_DATA</a> bind context parameter. <a href="https://msdn.microsoft.com/d89a0ee1-9a4b-48a4-8965-0d92f09743a6">STR_PARSE_PREFER_FOLDER_BROWSING</a> can be passed to indicate that URLs are parsed using the file system data source when possible. Construct a bind context object using <a href="https://msdn.microsoft.com/0f0ded09-7a7c-40bb-8198-b9f5058827d4">CreateBindCtx</a> and populate the values using <a href="https://msdn.microsoft.com/7ee2b5b2-9b9c-41f1-8e58-7432ebc0f9ed">IBindCtx::RegisterObjectParam</a>. See <b>Bind Context String Keys</b> for a complete list of these.



If no data is being passed to or received from the parsing function, this value can be <b>NULL</b>.


### -param pszDisplayName [in]

Type: <b>LPWSTR</b>

A null-terminated Unicode string with the display name. Because each Shell folder defines its own parsing syntax, the form this string can take may vary. The desktop folder, for instance, accepts paths such as "C:\My Docs\My File.txt". It also will accept references to items in the namespace that have a GUID associated with them using the "::{GUID}" syntax. For example, to retrieve a fully qualified identifier list for the control panel from the desktop folder, you can use the following:
    
                        

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>::{CLSID for Control Panel}\::{CLSID for printers folder}
</pre>
</td>
</tr>
</table></span></div>

### -param pchEaten [out]

Type: <b>ULONG*</b>

A pointer to a <b>ULONG</b> value that receives the number of characters of the display name that was parsed. If your application does not need this information, set <i>pchEaten</i> to <b>NULL</b>, and no value will be returned.


### -param ppidl [out]

Type: <b>PIDLIST_RELATIVE*</b>

When this method returns, contains a pointer to the PIDL for the object. The returned item identifier list specifies the item relative to the parsing folder. If the object associated with <i>pszDisplayName</i> is within the parsing folder, the returned item identifier list will contain only one <a href="https://msdn.microsoft.com/794c8425-2319-4339-881c-c5083ab05638">SHITEMID</a> structure. If the object is in a subfolder of the parsing folder, the returned item identifier list will contain multiple <b>SHITEMID</b> structures. If an error occurs, <b>NULL</b> is returned in this address.
                        

When it is no longer needed, it is the responsibility of the caller to free this resource by calling <a href="https://msdn.microsoft.com/3d0af12e-fc74-4ef7-b2dd-e9da5d0483c7">CoTaskMemFree</a>.


### -param pdwAttributes [in, out]

Type: <b>ULONG*</b>

The value used to query for file attributes. If not used, it should be set to <b>NULL</b>. To query for one or more attributes, initialize this parameter with the <a href="https://msdn.microsoft.com/4cb85995-cdc8-4474-8c4d-c783ac91c759">SFGAO</a> flags that represent the attributes of interest. On return, those attributes that are true <i>and</i> were requested will be set.




## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Some Shell folders may not implement <b>IShellFolder::ParseDisplayName</b>. Each folder that does will define its own parsing syntax.

<b>ParseDisplayName</b> is not expected to handle the relative path or parent folder indicators (".\" or "..\"). It is up to the caller to remove these appropriately.

Do not use the SFGAO_VALIDATE flag in <i>pdwAttributes</i> to verify the existence of the item whose name is being parsed. <b>IShellFolder::ParseDisplayName</b> implicitly validates the existence of the item unless that behavior is overridden by a special bind context parameter.

Querying for some attributes may be relatively slow and use significant amounts of memory. For example, to determine if a file is shared, the Shell will load network components. This procedure may require the loading of several DLLs. The purpose of <i>pdwAttributes</i> is to allow you to restrict the query to only that information that is needed. The following code fragment illustrates how to find out if a file is compressed.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>LPITEMIDLIST pidl;
ULONG cbEaten;
DWORD dwAttribs = SFGAO_COMPRESSED;

hres = psf-&gt;ParseDisplayName(NULL,
                             NULL,
                             lpwszDisplayName,
                             &amp;cbEaten,  // This can be NULL
                             &amp;pidl,
                             &amp;dwAttribs);

if(dwAttribs &amp; SFGAO_COMPRESSED)
{
    // Do something with the compressed file
}
</pre>
</td>
</tr>
</table></span></div>
Since <i>pdwAttributes</i> is an in/out parameter, it should always be initialized. If you pass in an uninitialized value, some of the bits may be inadvertantly set. <b>IShellFolder::ParseDisplayName</b> will then query for the corresponding attributes, which may lead to undesirable delays or memory demands. If you do not wish to query for attributes, set <i>pdwAttributes</i> to <b>NULL</b> to avoid unpredictable behavior.

This method is similar to the <a href="https://msdn.microsoft.com/bf18320c-1ff3-4280-bd67-70f6c2998285">IParseDisplayName::ParseDisplayName</a> method.




## -see-also




<a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a>



<a href="https://msdn.microsoft.com/9b008034-3576-429e-b67c-e2222592ca46">IShellFolder2</a>



<a href="https://msdn.microsoft.com/3864b386-7653-4661-880c-e96c08ff0dbb">IShellFolder::GetAttributesOf</a>



<a href="https://msdn.microsoft.com/67982d28-27ce-4482-b588-10fec8143750">IShellLink</a>
 

 
