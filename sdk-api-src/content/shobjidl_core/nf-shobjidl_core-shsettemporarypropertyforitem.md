---
UID: NF:shobjidl_core.SHSetTemporaryPropertyForItem
title: SHSetTemporaryPropertyForItem function
author: windows-driver-content
description: Sets a temporary property for the specified item. A temporary property is kept in a read/write store that holds properties only for the lifetime of the IShellItem object, instead of writing them back into the item.
old-location: shell\SHSetTemporaryPropertyForItem.htm
old-project: shell
ms.assetid: 779b1b2e-cd4b-404f-9d50-ac87b81640d2
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: SHSetTemporaryPropertyForItem, SHSetTemporaryPropertyForItem function [Windows Shell], _shell_SHSetTemporaryPropertyForItem, shell.SHSetTemporaryPropertyForItem, shobjidl_core/SHSetTemporaryPropertyForItem
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
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
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Shell32.dll
api_name:
-	SHSetTemporaryPropertyForItem
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# SHSetTemporaryPropertyForItem function


## -description


Sets a temporary property for the specified item. A temporary property is kept in a read/write store that holds properties only for the lifetime of the <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a> object, instead of writing them back into the item.


## -parameters




### -param psi [in]

Type: <b><a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>*</b>

A pointer to the item on which the temporary property is to be set.


### -param propkey [in]

Type: <b>REFPROPERTYKEY</b>

Reference to the <a href="https://msdn.microsoft.com/3f5f31af-f040-443b-9045-9761055381ea">PROPERTYKEY</a> that identifies the temporary property that is being set.


### -param propvar [in]

Type: <b>REFPROPVARIANT</b>

Reference to a <a href="https://msdn.microsoft.com/e86cc279-826d-4767-8d96-fc8280060ea1">PROPVARIANT</a> that contains the value of the temporary property.


## -returns



Type: <b>HRESULT</b>

If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



A temporary value can only be read with <a href="https://msdn.microsoft.com/53953a5a-04a2-4749-a03b-8cbd5ac889f1">SHGetTemporaryPropertyForItem</a> or by passing GPS_TEMPORARY to <a href="https://msdn.microsoft.com/706b2551-a9b0-4368-babb-e54cea6d297e">IShellItem2::GetPropertyStore</a>.


