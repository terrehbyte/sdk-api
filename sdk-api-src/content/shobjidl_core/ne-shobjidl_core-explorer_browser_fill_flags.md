---
UID: NE:shobjidl_core.EXPLORER_BROWSER_FILL_FLAGS
title: EXPLORER_BROWSER_FILL_FLAGS
author: windows-driver-content
description: These flags are used with IExplorerBrowser::FillFromObject.
old-location: shell\EXPLORER_BROWSER_FILL_FLAGS.htm
old-project: shell
ms.assetid: 5be62600-147d-4625-8e6c-aa6687da2168
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: EBF_NODROPTARGET, EBF_NONE, EBF_SELECTFROMDATAOBJECT, EXPLORER_BROWSER_FILL_FLAGS, EXPLORER_BROWSER_FILL_FLAGS enumeration [Windows Shell], _shell_EXPLORER_BROWSER_FILL_FLAGS, shell.EXPLORER_BROWSER_FILL_FLAGS, shobjidl_core/EBF_NODROPTARGET, shobjidl_core/EBF_NONE, shobjidl_core/EBF_SELECTFROMDATAOBJECT, shobjidl_core/EXPLORER_BROWSER_FILL_FLAGS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
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
req.typenames: EXPLORER_BROWSER_FILL_FLAGS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	shobjidl_core.h
api_name:
-	EXPLORER_BROWSER_FILL_FLAGS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Internet Explorer 6.01
---

# EXPLORER_BROWSER_FILL_FLAGS enumeration


## -description


These flags are used with <a href="https://msdn.microsoft.com/f978d5d1-a597-4e49-9a2a-de23e99bf65e">IExplorerBrowser::FillFromObject</a>.


## -enum-fields




### -field EBF_NONE

No flags.


### -field EBF_SELECTFROMDATAOBJECT

Causes <a href="https://msdn.microsoft.com/f978d5d1-a597-4e49-9a2a-de23e99bf65e">IExplorerBrowser::FillFromObject</a> to first populate the results folder with the contents of the parent folders of the items in the data object, and then select only the items that are in the data object.


### -field EBF_NODROPTARGET

Do not allow dropping on the folder. In other words, do not register a drop target for the view. Applications can then register their own drop targets.
