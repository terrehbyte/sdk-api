---
UID: NF:tapi3if.ITPluggableTerminalClassInfo.get_Version
title: ITPluggableTerminalClassInfo::get_Version
author: windows-driver-content
description: The get_Version method gets the terminal version.
old-location: tapi3\itpluggableterminalclassinfo_get_version.htm
old-project: Tapi
ms.assetid: e87ebf36-dace-4318-8d45-87f7a451284e
ms.author: windowsdriverdev
ms.date: 5/18/2018
ms.keywords: ITPluggableTerminalClassInfo interface [TAPI 2.2],get_Version method, ITPluggableTerminalClassInfo.get_Version, ITPluggableTerminalClassInfo::get_Version, _tapi3_itpluggableterminalclassinfo_get_version, get_Version, get_Version method [TAPI 2.2], get_Version method [TAPI 2.2],ITPluggableTerminalClassInfo interface, tapi3.itpluggableterminalclassinfo_get_version, tapi3if/ITPluggableTerminalClassInfo::get_Version
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: tapi3if.h
req.include-header: Tapi3.h
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
req.typenames: TERMINAL_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	Tapi3.dll
api_name:
-	ITPluggableTerminalClassInfo.get_Version
product: Windows
targetos: Windows
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
req.product: Windows XP with SP1 and later
---

# ITPluggableTerminalClassInfo::get_Version


## -description


The 
<b>get_Version</b> method gets the terminal version.


## -parameters




### -param pVersion [out]

 The <b>BSTR</b> representation of the terminal version. The <b>BSTR</b> is allocated using 
<a href="9e0437a2-9b4a-4576-88b0-5cb9d08ca29b">SysAllocString</a>. The <b>BSTR</b> argument should be deallocated by the client.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/0f7190c4-c696-4749-82f2-20fdbc8651f4">ITPluggableTerminalClassInfo</a>
 

 
