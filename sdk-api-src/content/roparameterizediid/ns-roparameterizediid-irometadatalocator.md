---
UID: NS:roparameterizediid.IRoMetaDataLocator
title: IRoMetaDataLocator
author: windows-driver-content
description: Enables the RoGetParameterizedTypeInstanceIID function to access run-time metadata.
old-location: winrt\irometadatalocator_struct.htm
old-project: WinRT
ms.assetid: A1004454-1C9F-46AF-8C88-BB8204FA0410
ms.author: windowsdriverdev
ms.date: 5/15/2018
ms.keywords: IRoMetaDataLocator, IRoMetaDataLocator structure [Windows Runtime], PIRoMetaDataLocator, PIRoMetaDataLocator structure pointer [Windows Runtime], roparameterizediid/IRoMetaDataLocator, roparameterizediid/PIRoMetaDataLocator, winrt.irometadatalocator_struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: roparameterizediid.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
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
-	HeaderDef
api_location:
-	roparameterizediid.h
api_name:
-	IRoMetaDataLocator
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# IRoMetaDataLocator structure


## -description


Enables the <a href="https://msdn.microsoft.com/DE908C82-5D7C-415C-B08B-31786589979B">RoGetParameterizedTypeInstanceIID</a> function to access run-time metadata.

Implement <b>IRoMetaDataLocator</b> when you're implementing programming language bindings to enable a language to call Windows platform APIs by using Windows metadata (.winmd) files.




## -struct-fields






#### - Locate

Gets a metadata builder for the specified type.



#### nameElement

A Windows Runtime type or parameterized type to resolve.



#### metaDataDestination

A data sink for Windows Runtime metadata. The caller should invoke the appropriate set method to provide the metadata for the type named by <i>nameElement</i>.


## -see-also




<a href="https://msdn.microsoft.com/FF4FEA9F-3FB0-4D56-BE9A-E8E2CB13D718">RoGetMetaDataFile</a>
 

 
