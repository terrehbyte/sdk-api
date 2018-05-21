---
UID: NF:shobjidl_core.ITransferSource.SetProperties
title: ITransferSource::SetProperties
author: windows-driver-content
description: Sets properties that should be applied to an item.
old-location: shell\ITransferSource_SetProperties.htm
old-project: shell
ms.assetid: c42497cc-5a19-41da-9356-1086796032a7
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ITransferSource interface [Windows Shell],SetProperties method, ITransferSource.SetProperties, ITransferSource::SetProperties, SetProperties, SetProperties method [Windows Shell], SetProperties method [Windows Shell],ITransferSource interface, _shell_ITransferSource_SetProperties, shell.ITransferSource_SetProperties, shobjidl_core/ITransferSource::SetProperties
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
-	ITransferSource.SetProperties
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ITransferSource::SetProperties


## -description


Sets properties that should be applied to an item.


## -parameters




### -param pproparray [in]

Type: <b><a href="https://msdn.microsoft.com/c7de40d0-9fe6-4c4b-ba17-c4648501ce0a">IPropertyChangeArray</a>*</b>

An array of properties and their changed values.


## -returns



Type: <b>HRESULT</b>

Any return value other than S_OK indicates a failure.


