---
UID: NF:shobjidl_core.IApplicationAssociationRegistration.SetAppAsDefaultAll
title: IApplicationAssociationRegistration::SetAppAsDefaultAll
author: windows-driver-content
description: Sets an application as the default for all of the registered associations of any type for that application. Not intended for use in Windows 8.
old-location: shell\IApplicationAssociationRegistration_SetAppAsDefaultAll.htm
old-project: shell
ms.assetid: 3e9ad8ba-0f0e-46e6-ab0b-61c35bfd2dc6
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IApplicationAssociationRegistration interface [Windows Shell],SetAppAsDefaultAll method, IApplicationAssociationRegistration.SetAppAsDefaultAll, IApplicationAssociationRegistration::SetAppAsDefaultAll, SetAppAsDefaultAll, SetAppAsDefaultAll method [Windows Shell], SetAppAsDefaultAll method [Windows Shell],IApplicationAssociationRegistration interface, _shell_IApplicationAssociationRegistration_SetAppAsDefaultAll, shell.IApplicationAssociationRegistration_SetAppAsDefaultAll, shobjidl_core/IApplicationAssociationRegistration::SetAppAsDefaultAll
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
-	IApplicationAssociationRegistration.SetAppAsDefaultAll
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IApplicationAssociationRegistration::SetAppAsDefaultAll


## -description


Sets an application as the default for all of the registered associations of any <a href="https://msdn.microsoft.com/library/windows/hardware/hh439450">type</a> for that application. Not intended for use in Windows 8.


## -parameters




### -param pszAppRegistryName [in]

Type: <b>LPCWSTR</b>

A pointer to a null-terminated Unicode string that specifies the registered name of the application.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/78cd05a4-df33-42b5-91b9-826ebce04a1d">Default Programs</a>



<a href="https://msdn.microsoft.com/015a3be4-2e74-4a2b-8c02-54dcbf0ecacd">IApplicationAssociationRegistration</a>
 

 
