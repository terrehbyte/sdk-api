---
UID: NF:winsxs.IAssemblyCacheItem.CreateStream
title: IAssemblyCacheItem::CreateStream
author: windows-driver-content
description: The CreateStream method copies the source of a manifest or module into a stream.
old-location: setup\iassemblycacheitem_createstream.htm
old-project: SbsCs
ms.assetid: 3b3726cc-91c2-4614-a3a7-3f89f201e04a
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: CreateStream, CreateStream method [Side-by-side Assemblies], CreateStream method [Side-by-side Assemblies],IAssemblyCacheItem interface, IAssemblyCacheItem interface [Side-by-side Assemblies],CreateStream method, IAssemblyCacheItem.CreateStream, IAssemblyCacheItem::CreateStream, STREAM_FORMAT_COMPLIB_MANIFEST, STREAM_FORMAT_COMPLIB_MODULE, STREAM_FORMAT_WIN32_MANIFEST, STREAM_FORMAT_WIN32_MODULE, setup.iassemblycacheitem_createstream, winsxs/IAssemblyCacheItem::CreateStream
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: winsxs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: CREATE_ASM_NAME_OBJ_FLAGS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	sxs.dll
api_name:
-	IAssemblyCacheItem.CreateStream
product: Windows
targetos: Windows
req.lib: 
req.dll: Sxs.dll
req.irql: 
req.product: Windows XP Professional x64 Edition or 64-bit editions of     Windows Server 2003
---

# IAssemblyCacheItem::CreateStream


## -description


The <b>CreateStream</b> method copies the source of a manifest or module into a stream.


## -parameters




### -param dwFlags [in]

Reserved.


### -param pszStreamName [in]

Pointer to a string value containing the name of the manifest. This becomes the name of the stream.


### -param dwFormat [in]

This parameter specifies whether a module or manifest is being copied to a stream.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="STREAM_FORMAT_COMPLIB_MODULE"></a><a id="stream_format_complib_module"></a><dl>
<dt><b>STREAM_FORMAT_COMPLIB_MODULE</b></dt>
</dl>
</td>
<td width="60%">
Copy  the source  of a module for a non-Windows assembly to a stream.

</td>
</tr>
<tr>
<td width="40%"><a id="STREAM_FORMAT_COMPLIB_MANIFEST"></a><a id="stream_format_complib_manifest"></a><dl>
<dt><b>STREAM_FORMAT_COMPLIB_MANIFEST</b></dt>
</dl>
</td>
<td width="60%">
Copy  the source  of a manifest for a non-Windows assembly to a stream.

</td>
</tr>
<tr>
<td width="40%"><a id="STREAM_FORMAT_WIN32_MODULE"></a><a id="stream_format_win32_module"></a><dl>
<dt><b>STREAM_FORMAT_WIN32_MODULE</b></dt>
</dl>
</td>
<td width="60%">
Copy  the source  of a module for a Windows assembly to a stream.

</td>
</tr>
<tr>
<td width="40%"><a id="STREAM_FORMAT_WIN32_MANIFEST"></a><a id="stream_format_win32_manifest"></a><dl>
<dt><b>STREAM_FORMAT_WIN32_MANIFEST</b></dt>
</dl>
</td>
<td width="60%">
Copy  the source  of a manifest for a Windows assembly to a stream.

</td>
</tr>
</table>
 


### -param dwFormatFlags [in]

Reserved.


### -param ppIStream

Pointer to the location that contains the pointer to the IStream interface that receives the information.


### -param puliMaxSize [optional]

Reserved.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt>S_OK</dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt>S_FALSE</dt>
</dl>
</td>
<td width="60%">
The method did not succeed.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/9df9ee58-0354-49f0-af9c-5b92179cfaea">IAssemblyCacheItem</a>
 

 
