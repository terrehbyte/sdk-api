---
UID: NF:iwscapi.IWSCProductList.get_Count
title: IWSCProductList::get_Count
author: windows-sdk-content
description: Gathers the total number of all security product providers of the specified type on the computer.
old-location: winprog\iwscproductlist_count.htm
old-project: DevNotes
ms.assetid: A28A6D3B-DC11-418B-987F-04711358B6EE
ms.author: windowssdkdev
ms.date: 05/23/2018
ms.keywords: IWSCProductList interface [Windows API],get_Count method, IWSCProductList.get_Count, IWSCProductList::get_Count, get_Count, get_Count method [Windows API], get_Count method [Windows API],IWSCProductList interface, iwscapi/IWSCProductList::get_Count, winprog.iwscproductlist_count
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: iwscapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: WSC_SECURITY_SIGNATURE_STATUS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Wscapi.dll
api_name:
-	IWSCProductList.get_Count
product: Windows
targetos: Windows
req.lib: Wscapi.lib
req.dll: Wscapi.dll
req.irql: 
req.product: GDI+ 1.1
---

# IWSCProductList::get_Count


## -description


Gathers the total number of all security product providers of the specified type on the computer.


## -parameters




### -param pVal [out]

A pointer to the number of providers in the list of security products on the computer.


## -returns



If the method  succeeds, returns S_OK.

If the method  fails, returns a Win32 error code.




## -see-also




<a href="https://msdn.microsoft.com/81BC78F1-6F95-49D3-8EDD-EB7E13119A86">IWSCProductList</a>
 

 
