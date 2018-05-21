---
UID: NF:shobjidl_core.IExecuteCommand.SetDirectory
title: IExecuteCommand::SetDirectory
author: windows-driver-content
description: Sets a new working directory.
old-location: shell\IExecuteCommand_SetDirectory.htm
old-project: shell
ms.assetid: 8416b2ef-8e62-4679-adc1-ec953875db34
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IExecuteCommand interface [Windows Shell],SetDirectory method, IExecuteCommand.SetDirectory, IExecuteCommand::SetDirectory, SetDirectory, SetDirectory method [Windows Shell], SetDirectory method [Windows Shell],IExecuteCommand interface, _shell_IExecuteCommand_SetDirectory, shell.IExecuteCommand_SetDirectory, shobjidl_core/IExecuteCommand::SetDirectory
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
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
-	IExecuteCommand.SetDirectory
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IExecuteCommand::SetDirectory


## -description


Sets a new working directory.


## -parameters




### -param pszDirectory [in]

Type: <b>LPCWSTR</b>

Pointer to a null-terminated string with the fully qualified path of the new working directory. If this value is <b>NULL</b>, the current working directory is used.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


