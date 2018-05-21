---
UID: NF:shobjidl_core.ISharingConfigurationManager.ArePrintersShared
title: ISharingConfigurationManager::ArePrintersShared
author: windows-driver-content
description: Determines whether any printers connected to this computer are shared.
old-location: shell\ISharingConfigurationManager_ArePrintersShared.htm
old-project: shell
ms.assetid: 331ccf4d-c769-43b9-a2db-c464ffaef58e
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ArePrintersShared, ArePrintersShared method [Windows Shell], ArePrintersShared method [Windows Shell],ISharingConfigurationManager interface, ISharingConfigurationManager interface [Windows Shell],ArePrintersShared method, ISharingConfigurationManager.ArePrintersShared, ISharingConfigurationManager::ArePrintersShared, _shell_ISharingConfigurationManager_ArePrintersShared, shell.ISharingConfigurationManager_ArePrintersShared, shobjidl_core/ISharingConfigurationManager::ArePrintersShared
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
-	shobjidl_core.h
api_name:
-	ISharingConfigurationManager.ArePrintersShared
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ISharingConfigurationManager::ArePrintersShared


## -description


Determines whether any printers connected to this computer are shared.


## -parameters






## -returns



Type: <b>HRESULT</b>

Returns standard HRESULT values, including the following:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Shared printers were detected.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
No shared printers were found.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_FILE_NOT_FOUND</b></dt>
</dl>
</td>
<td width="60%">
No printers capable of being shared were found.

</td>
</tr>
</table>
 


