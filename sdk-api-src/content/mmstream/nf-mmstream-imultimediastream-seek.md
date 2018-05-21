---
UID: NF:mmstream.IMultiMediaStream.Seek
title: IMultiMediaStream::Seek
author: windows-driver-content
description: Note  This interface is deprecated. New applications should not use it. The Seek method seeks all of the media streams to a new position.
old-location: dshow\imultimediastream_seek.htm
old-project: DirectShow
ms.assetid: ac65613f-3fca-4043-83ad-740ebd7687a4
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IMultiMediaStream interface [DirectShow],Seek method, IMultiMediaStream.Seek, IMultiMediaStream::Seek, IMultiMediaStreamSeek, Seek, Seek method [DirectShow], Seek method [DirectShow],IMultiMediaStream interface, dshow.imultimediastream_seek, mmstream/IMultiMediaStream::Seek
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mmstream.h
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
req.typenames: STREAM_STATE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	mmstream.h
api_name:
-	IMultiMediaStream.Seek
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: GDI+ 1.1
---

# IMultiMediaStream::Seek


## -description



<div class="alert"><b>Note</b>  This interface is deprecated. New applications should not use it.</div>
<div> </div>
The <code>Seek</code> method seeks all of the media streams to a new position.




## -parameters




### -param SeekTime [in]


<a href="https://msdn.microsoft.com/eff79c58-09d8-4665-9138-752ffaf02e26">STREAM_TIME</a> value that specifies the new position.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_NOINTERFACE</b></dt>
</dl>
</td>
<td width="60%">
The media streams do not support seeking.

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



To determine whether the media streams support seeking, call the <a href="https://msdn.microsoft.com/27be6104-9ca4-48d7-aeda-5b633460e252">IMultiMediaStream::GetInformation</a> method.




## -see-also




<a href="https://msdn.microsoft.com/8be6c74f-9290-48b4-ad66-8d7d7cc94174">IMultiMediaStream Interface</a>
 

 
