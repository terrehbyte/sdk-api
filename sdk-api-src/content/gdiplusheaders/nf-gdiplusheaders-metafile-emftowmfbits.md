---
UID: NF:gdiplusheaders.Metafile.EmfToWmfBits
title: Metafile::EmfToWmfBits
author: windows-driver-content
description: Converts an enhanced-format metafile to a Windows Metafile Format (WMF) metafile and stores the converted records in a specified buffer.
old-location: gdiplus\_gdiplus_CLASS_Metafile_EmfToWmfBits_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\metafileclass\metafilemethods\emftowmfbits.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: EmfToWmfBits, EmfToWmfBits method [GDI+], EmfToWmfBits method [GDI+],Metafile class, Metafile class [GDI+],EmfToWmfBits method, Metafile.EmfToWmfBits, Metafile::EmfToWmfBits, _gdiplus_CLASS_Metafile_EmfToWmfBits_, gdiplus._gdiplus_CLASS_Metafile_EmfToWmfBits_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdiplusheaders.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
-	Gdiplus.dll
api_name:
-	Metafile.EmfToWmfBits
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Metafile::EmfToWmfBits


## -description


Converts an enhanced-format metafile to a Windows Metafile Format (WMF) metafile and stores the converted records in a specified buffer. 




## -parameters




### -param hemf [in]

Type: <b>HENHMETAFILE</b>

Handle to the enhanced-format metafile that is to be converted.


### -param cbData16 [in]

Type: <b>UINT</b>

Unsigned integer that specifies the number of bytes in the buffer pointed to by the <i>pData16</i> parameter.


### -param pData16 [out]

Type: <b>LPBYTE</b>

Pointer to a buffer that receives the converted records. If <i>pData16</i> is <b>NULL</b>, <b>Metafile::EmfToWmfBits</b> returns the number of bytes required to store the converted metafile records.


### -param iMapMode [in, optional]

Type: <b>INT</b>

Optional. Specifies the mapping mode to use in the converted metafile. For a list of possible mapping modes, see <a href="https://msdn.microsoft.com/a4d6a63a-6d2d-4bd9-9e71-4cd1b5f145a4">SetMapMode</a>. The default value is MM_ANISOTROPIC.


### -param eFlags [in, optional]

Type: <b><a href="https://msdn.microsoft.com/b45a2569-a1f8-4888-9dcd-518373f1ceb1">EmfToWmfBitsFlags</a></b>

Optional. Element of the <a href="https://msdn.microsoft.com/b45a2569-a1f8-4888-9dcd-518373f1ceb1">EmfToWmfBitsFlags</a> enumeration that specifies options for the conversion. The default value is <a href="https://msdn.microsoft.com/b45a2569-a1f8-4888-9dcd-518373f1ceb1">EmfToWmfBitsFlagsDefault</a>.


## -returns



Type: <strong>Type: <b>UINT</b>
</strong>

If the method succeeds and the buffer pointer is <b>NULL</b>, the return value is the number of bytes required to store the converted records. If the method succeeds and the buffer pointer is a valid pointer, the return value is the size of the metafile data in bytes. If the method fails, the return value is zero.




## -remarks



When you call <b>Metafile::EmfToWmfBits</b> to determine the size of the required buffer, you must pass the same value for <i>eFlags</i> that you pass later when you call <b>Metafile::EmfToWmfBits</b> to perform the conversion. Otherwise, the size returned by the first call to <b>Metafile::EmfToWmfBits</b> will be incorrect.

This method cannot convert metafiles of type <a href="https://msdn.microsoft.com/b45a2569-a1f8-4888-9dcd-518373f1ceb1">EmfTypeEmfPlusOnly</a>. If you use this method to convert a metafile of type <a href="https://msdn.microsoft.com/b45a2569-a1f8-4888-9dcd-518373f1ceb1">EmfTypeEmfPlusDual</a>, the Enhanced Metafile (EMF) records in that metafile are converted, but the EMF+ records are not converted.

This method converts an enhanced metafile into a WMF metafile so that its picture can be displayed in an application that recognizes the older format.

The <b>Metafile::EmfToWmfBits</b> method does not invalidate the enhanced metafile handle. Call the <a href="https://msdn.microsoft.com/d3b93b3b-fa0b-4480-8348-19919c9e904d">DeleteEnhMetaFile</a> function to release the handle when it is no longer needed.

To create a scalable WMF metafile, specify MM_ANISOTROPIC as the <i>iMapMode</i> parameter.


#### Examples




			The following example converts an enhanced-format metafile to a WMF metafile. The last parameter passed to <b>Metafile::EmfToWmfBits</b> specifies that the enhanced-format metafile is embedded as a comment in the converted metafile.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>// Construct a Metafile object from an existing EMF disk file.
Metafile myMetafile(L"SourceMetafile.emf");

// Get a handle to the EMF metafile.
HENHMETAFILE hEmf = myMetafile.GetHENHMETAFILE();

// Determine the size of the buffer that will receive the converted records.
UINT size = Metafile::EmfToWmfBits(
   hEmf, 
   0, 
   NULL,
   MM_ANISOTROPIC,
   EmfToWmfBitsFlagsEmbedEmf);

// Allocate a buffer to receive the converted records.
BYTE* buffer = new BYTE[size];

// Convert the EMF records to WMF records.
INT convertedSize = Metafile::EmfToWmfBits(
   hEmf, 
   size,
   buffer, 
   MM_ANISOTROPIC,
   EmfToWmfBitsFlagsEmbedEmf);

// Get a handle to the converted metafile.
HMETAFILE hmf = SetMetaFileBitsEx(size, buffer);

// Write the WMF metafile to a disk file.
CopyMetaFile(hmf, TEXT("ConvertedMetafile.wmf"));

DeleteMetaFile(hmf);
DeleteEnhMetaFile(hEmf);
delete[] buffer;</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/985c412f-10ba-4ce9-b0e1-89f5b643c22a">EmfType</a>



<a href="https://msdn.microsoft.com/db61ea3a-44d0-4769-acb4-05a982d3f06f">GetWinMetaFileBits</a>



<a href="https://msdn.microsoft.com/63b057de-9c4d-488e-ad07-ede52f9175a6">Metafile</a>



<a href="https://msdn.microsoft.com/a9f9bac4-f3c7-44a1-9f0f-59ff1a27b077">Metafiles</a>
 

 
