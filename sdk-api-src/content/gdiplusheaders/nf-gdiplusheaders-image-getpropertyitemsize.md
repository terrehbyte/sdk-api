---
UID: NF:gdiplusheaders.Image.GetPropertyItemSize
title: Image::GetPropertyItemSize
author: windows-driver-content
description: The Image::GetPropertyItemSize method gets the size, in bytes, of a specified property item of this Image object.
old-location: gdiplus\_gdiplus_CLASS_Image_GetPropertyItemSize_propId_.htm
old-project: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\imageclass\imagemethods\getpropertyitemsize.htm
ms.author: windowsdriverdev
ms.date: 5/14/2018
ms.keywords: GetPropertyItemSize, GetPropertyItemSize method [GDI+], GetPropertyItemSize method [GDI+],Image class, Image class [GDI+],GetPropertyItemSize method, Image.GetPropertyItemSize, Image::GetPropertyItemSize, _gdiplus_CLASS_Image_GetPropertyItemSize_propId_, gdiplus._gdiplus_CLASS_Image_GetPropertyItemSize_propId_
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
-	Image.GetPropertyItemSize
product: Windows
targetos: Windows
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
req.product: GDI+ 1.0
---

# Image::GetPropertyItemSize


## -description


The <b>Image::GetPropertyItemSize</b> method gets the size, in bytes, of a specified property item of this 
			<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a> object.


## -parameters




### -param propId [in]

Type: <b>PROPID</b>

Integer that identifies the property item. 


## -returns



Type: <strong>Type: <b>UINT</b>
</strong>

This method returns the size, in bytes, of a specified property item of this 
						<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a> object.




## -remarks



The <a href="https://msdn.microsoft.com/ca96c4a3-058f-4ba4-a8be-2692ecd76710">Image::GetPropertyItem</a> method returns a <a href="https://msdn.microsoft.com/449f8ba0-0c94-4733-80e1-1c03819e4c39">PropertyItem</a> object. Before you call 
				<b>Image::GetPropertyItem</b>, you must allocate a buffer large enough to receive that object — the size varies according to data type and value of the property item. You can call the <b>Image::GetPropertyItemSize</b> method of an 
				<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a> object to get the size, in bytes, of the required buffer.


#### Examples




			The following example creates an 
						<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a> object based on a JPEG file. The code calls the <b>Image::GetPropertyItemSize</b> method of that 
						<b>Image</b> object to get the size of the property item that holds the make of the camera used to capture the image. Then the code calls the <a href="https://msdn.microsoft.com/ca96c4a3-058f-4ba4-a8be-2692ecd76710">Image::GetPropertyItem</a> method to retrieve that property item.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>#include &lt;windows.h&gt;
#include &lt;gdiplus.h&gt;
#include &lt;stdio.h&gt;
using namespace Gdiplus;

INT main()
{
   GdiplusStartupInput gdiplusStartupInput;
   ULONG_PTR gdiplusToken;
   GdiplusStartup(&amp;gdiplusToken, &amp;gdiplusStartupInput, NULL);

   UINT size = 0;
   PropertyItem* propertyItem = NULL;
   Image* image = new Image(L"FakePhoto.jpg");

   // Assume that the image has a property item of type PropertyItemEquipMake.
   // Get the size of that property item.
   size = image-&gt;GetPropertyItemSize(PropertyTagEquipMake);

   // Allocate a buffer to receive the property item.
   propertyItem = (PropertyItem*)malloc(size);

   // Get the property item.
   image-&gt;GetPropertyItem(PropertyTagEquipMake, size, propertyItem);

   // Display the members of the retrieved PropertyItem object.
   printf("The length of the property item is %u.\n", propertyItem-&gt;length);
   printf("The data type of the property item is %u.\n", propertyItem-&gt;type);

   if(propertyItem-&gt;type == PropertyTagTypeASCII)
      printf("The value of the property item is %s.\n", propertyItem-&gt;value);

   free(propertyItem);
   delete image;
   GdiplusShutdown(gdiplusToken);
   return 0;
}</pre>
</td>
</tr>
</table></span></div>
The preceding code, along with a particular file, FakePhoto.jpg, produced the following output. Note that the data type is 2, which is the value of the PropertyTagTypeASCII constant that is defined in Gdiplusimaging.h.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>The length of the property item is 17.
The data type of the property item is 2.
The value of the property item is Northwind Traders.</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/3732095d-c812-4ce5-80f1-9b191b4ff01c">Image</a>



<a href="https://msdn.microsoft.com/c22c2027-9552-4f35-ba44-755d872ceea7">Image::GetAllPropertyItems</a>



<a href="https://msdn.microsoft.com/fff3acf1-2a2f-46b6-af7e-02b7ef52bb40">Image::GetPropertyCount</a>



<a href="https://msdn.microsoft.com/2318eb42-9006-4361-ac5c-4e5325dc4947">Image::GetPropertyIdList</a>



<a href="https://msdn.microsoft.com/ca96c4a3-058f-4ba4-a8be-2692ecd76710">Image::GetPropertyItem</a>



<a href="https://msdn.microsoft.com/731c0d1a-1918-4db8-ace1-e8a42cdefa3d">Image::GetPropertySize</a>



<a href="https://msdn.microsoft.com/ad849843-80e7-4773-96b0-f50dbdbfd61b">Image::RemovePropertyItem</a>



<a href="https://msdn.microsoft.com/20201f1e-fa80-4a7b-b7cc-7737d4a434a5">Image::SetPropertyItem</a>



<a href="https://msdn.microsoft.com/449f8ba0-0c94-4733-80e1-1c03819e4c39">PropertyItem</a>



<a href="https://msdn.microsoft.com/2febea35-3fea-4a2d-baaf-7a4f935fc81f">Reading and Writing Metadata</a>
 

 
