---
UID: NF:shobjidl_core.IPropertyUI.GetHelpInfo
title: IPropertyUI::GetHelpInfo
author: windows-driver-content
description: Developers should use IPropertyDescription instead.
old-location: properties\IPropertyUI_GetHelpInfo.htm
old-project: properties
ms.assetid: 165ABA55-7CDB-48cf-AE14-DA314197BA42
ms.author: windowsdriverdev
ms.date: 5/8/2018
ms.keywords: GetHelpInfo, GetHelpInfo method [Windows Properties], GetHelpInfo method [Windows Properties],IPropertyUI interface, IPropertyUI interface [Windows Properties],GetHelpInfo method, IPropertyUI.GetHelpInfo, IPropertyUI::GetHelpInfo, _shell_IPropertyUI_GetHelpInfo, properties.IPropertyUI_GetHelpInfo, shell.IPropertyUI_GetHelpInfo, shobjidl_core/IPropertyUI::GetHelpInfo
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
-	Shobjidl_core.h
api_name:
-	IPropertyUI.GetHelpInfo
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IPropertyUI::GetHelpInfo


## -description


Developers should use <a href="shell.IPropertyDescription">IPropertyDescription</a> instead. Gets


## -parameters




### -param fmtid [in]

Type: <b>REFFMTID</b>

The FMTID of the property.


### -param pid [in]

Type: <b>PROPID</b>

The PROPID of the property.


### -param pwszHelpFile [out]

Type: <b>LPWSTR</b>

The fully qualified path of the Help file.


### -param cch [in]

Type: <b>DWORD</b>


### -param puHelpID [out]

Type: <b>UINT*</b>

The Help context ID for the property.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


