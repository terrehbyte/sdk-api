---
UID: NF:fileapi.FindNextFileNameW
title: FindNextFileNameW function
author: windows-driver-content
description: Continues enumerating the hard links to a file using the handle returned by a successful call to the FindFirstFileNameW function.
old-location: fs\findnextfilenamew.htm
old-project: FileIO
ms.assetid: 1d2f8041-2744-4f37-afde-ddce49a8bdc5
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: FindNextFileNameW, FindNextFileNameW function [Files], fileapi/FindNextFileNameW, fs.findnextfilenamew
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: fileapi.h
req.include-header: Windows.h, WinBase.h
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
req.typenames: STREAM_INFO_LEVELS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Kernel32.dll
-	API-MS-Win-Core-File-L1-2-2.dll
-	KernelBase.dll
api_name:
-	FindNextFileNameW
product: Windows
targetos: Windows
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
req.product: Internet Explorer 5
---

# FindNextFileNameW function


## -description


Continues enumerating the hard links to a file using the handle returned by a successful call to the 
    <a href="https://msdn.microsoft.com/9f64aa3e-4c73-47a8-8304-6134f1b4d153">FindFirstFileNameW</a> function.


## -parameters




### -param hFindStream [in]

A handle to the enumeration that is returned by a successful call to 
      <a href="https://msdn.microsoft.com/9f64aa3e-4c73-47a8-8304-6134f1b4d153">FindFirstFileNameW</a>.


### -param StringLength [in, out]

The size of the <i>LinkName</i> parameter, in characters. If this call fails and the 
      error is <b>ERROR_MORE_DATA</b>, the value that is returned by this parameter is the size 
      that <i>LinkName</i>  must be to contain all the data.


### -param LinkName [in, out]

A pointer to a buffer to store the first link name found for <i>lpFileName</i>.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero (0). To get extended error information, call 
       <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a>.

If no matching files can be found, the <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> 
       function returns <b>ERROR_HANDLE_EOF</b>.




## -remarks



If the function returns <b>TRUE</b>, there are more hard links to enumerate.

In Windows 8 and Windows Server 2012, this function is supported by the following technologies.

<table>
<tr>
<th>Technology</th>
<th>Supported</th>
</tr>
<tr>
<td>
Server Message Block (SMB) 3.0 protocol

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
SMB 3.0 Transparent Failover (TFO)

</td>
<td>
No

</td>
</tr>
<tr>
<td>
SMB 3.0 with Scale-out File Shares (SO)

</td>
<td>
No

</td>
</tr>
<tr>
<td>
Cluster Shared Volume File System (CsvFS)

</td>
<td>
Yes

</td>
</tr>
<tr>
<td>
Resilient File System (ReFS)

</td>
<td>
Yes

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/1cf0547d-54ac-410a-acbe-7b3b3ebb310b">File Management Functions</a>



<a href="https://msdn.microsoft.com/64b3bc49-1e0e-4572-9d9f-936c45f5b01c">FindClose</a>



<a href="https://msdn.microsoft.com/9f64aa3e-4c73-47a8-8304-6134f1b4d153">FindFirstFileNameW</a>
 

 
