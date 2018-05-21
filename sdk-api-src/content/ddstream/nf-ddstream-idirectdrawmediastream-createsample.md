---
UID: NF:ddstream.IDirectDrawMediaStream.CreateSample
title: IDirectDrawMediaStream::CreateSample
author: windows-driver-content
description: Note  This interface is deprecated. New applications should not use it. Creates a stream sample using the specified DirectDraw surface object.
old-location: dshow\idirectdrawmediastream_createsample.htm
old-project: DirectShow
ms.assetid: 85041c71-f9fc-48fc-8fe2-fec21efb831b
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: CreateSample, CreateSample method [DirectShow], CreateSample method [DirectShow],IDirectDrawMediaStream interface, IDirectDrawMediaStream interface [DirectShow],CreateSample method, IDirectDrawMediaStream.CreateSample, IDirectDrawMediaStream::CreateSample, IDirectDrawMediaStreamCreateSample, ddstream/IDirectDrawMediaStream::CreateSample, dshow.idirectdrawmediastream_createsample
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: ddstream.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: VIDEOMEMORYINFO
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	ddstream.h
api_name:
-	IDirectDrawMediaStream.CreateSample
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# IDirectDrawMediaStream::CreateSample


## -description



<div class="alert"><b>Note</b>  This interface is deprecated. New applications should not use it.</div>
<div> </div>
Creates a stream sample using the specified DirectDraw surface object.




## -parameters




### -param pSurface [in]

Pointer to an existing DirectDraw surface. Use <b>QueryInterface</b> to obtain the <b>IDirectDrawSurface</b> interface from an <b>IDirectDrawSurface7</b> interface pointer.


### -param pRect [in]

Pointer to the clipping rectangle you want to use with the specified surface. Set this parameter to <b>NULL</b> if you want to use the entire surface.


### -param dwFlags [in]

Specifies miscellaneous flags. The following flag is defined:

<table>
<tr>
<th>
                  Value
                </th>
<th>
                  Description
                </th>
</tr>
<tr>
<td>DDSFF_PROGRESSIVERENDER</td>
<td>If this flag is set, sample updates are performed directly on the surface. When this flag is absent, if the decoder uses delta frames, an extra copy is performed internally. Setting this flag can improve performance but can also introduce tearing.</td>
</tr>
</table>
 


### -param ppSample [out]

Address of a pointer to an <a href="https://msdn.microsoft.com/afc8ac84-4629-4c5d-b4b2-59c1eb1af35d">IDirectDrawStreamSample</a> interface that will point to the newly created sample.


## -returns



Returns one of the following values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DDERR_INVALIDPIXELFORMAT</b></dt>
</dl>
</td>
<td width="60%">
The specified pixel format is incompatible with the stream format.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DDERR_INVALIDRECT</b></dt>
</dl>
</td>
<td width="60%">
The specified clipping rectangle is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>DDERR_INVALIDSURFACETYPE</b></dt>
</dl>
</td>
<td width="60%">
The specified surface is incompatible with the stream format.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
One or more of the required parameters is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MS_E_SAMPLEALLOC</b></dt>
</dl>
</td>
<td width="60%">
The stream already has allocated samples and the surface doesn't match the sample format.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
</table>
 




## -remarks



This method creates a sample from the current stream and attaches the sample to this surface.

If the stream doesn't have an allocated surface and the specified surface doesn't match the stream's format, this method calls the <a href="https://msdn.microsoft.com/465b4f0c-40e1-4aec-be62-0b55c29fa05e">IDirectDrawMediaStream::SetFormat</a> method on the stream so the two will match.

To perform a progressive render, create a single sample and repeatedly use that sample for successive frames of video. Video decompressors use this technique to do partial updates to the previous frame.

The <i>pRect</i> parameter should match the format of the stream (see <a href="https://msdn.microsoft.com/3729bbe6-3504-46b3-9978-e66afc56344f">IDirectDrawMediaStream::GetFormat</a>). If the wrong clip rectangle is set or no clip rectangle is set, and the surface size does not match the movie size, the movie might not play. If a primary surface is used, it is advisable to use a clipping rectangle because the primary surface size can change if the user changes display settings.




## -see-also




<a href="https://msdn.microsoft.com/858af0c3-9e22-45d8-ab08-307eb39a8977">IDirectDrawMediaStream Interface</a>
 

 
