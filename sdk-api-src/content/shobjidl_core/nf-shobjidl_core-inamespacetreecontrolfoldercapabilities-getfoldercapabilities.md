---
UID: NF:shobjidl_core.INameSpaceTreeControlFolderCapabilities.GetFolderCapabilities
title: INameSpaceTreeControlFolderCapabilities::GetFolderCapabilities
author: windows-driver-content
description: Gets a folder's capability to be filtered through the System.IsPinnedToNameSpaceTree property key value and change notification registration status.
old-location: shell\INameSpaceTreeControlFolderCapabilities_GetFolderCapabilities.htm
old-project: shell
ms.assetid: 1534431c-21fc-4eb9-8f17-ddd7414bef94
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: GetFolderCapabilities, GetFolderCapabilities method [Windows Shell], GetFolderCapabilities method [Windows Shell],INameSpaceTreeControlFolderCapabilities interface, INameSpaceTreeControlFolderCapabilities interface [Windows Shell],GetFolderCapabilities method, INameSpaceTreeControlFolderCapabilities.GetFolderCapabilities, INameSpaceTreeControlFolderCapabilities::GetFolderCapabilities, NSTCFC_DELAY_REGISTER_NOTIFY, NSTCFC_NONE, NSTCFC_PINNEDITEMFILTERING, _shell_INameSpaceTreeControlFolderCapabilities_GetFolderCapabilities, shell.INameSpaceTreeControlFolderCapabilities_GetFolderCapabilities, shobjidl_core/INameSpaceTreeControlFolderCapabilities::GetFolderCapabilities
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
-	INameSpaceTreeControlFolderCapabilities.GetFolderCapabilities
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# INameSpaceTreeControlFolderCapabilities::GetFolderCapabilities


## -description


Gets a folder's capability to be filtered through the <a href="https://msdn.microsoft.com/00937acb-1ce2-44f6-96a1-69e5dbb665f6">System.IsPinnedToNameSpaceTree</a> property key value and change notification registration status.


## -parameters




### -param nfcMask [in]

Type: <b><a href="https://msdn.microsoft.com/a5282277-85f5-494e-b994-efbf1116b519">NSTCFOLDERCAPABILITIES</a></b>

The capabilities for which this method should retrieve values. Specify one or both of the following:



#### NSTCFC_PINNEDITEMFILTERING (0x00000001)

0x00000001. The <a href="https://msdn.microsoft.com/00937acb-1ce2-44f6-96a1-69e5dbb665f6">System.IsPinnedToNameSpaceTree</a> property exists on this folder and filtering based on that property value is supported.



#### NSTCFC_DELAY_REGISTER_NOTIFY (0x00000002)

0x00000002. Registration for change notifications is delayed until the folder is expanded in the navigation pane.


### -param pnfcValue






#### - pnstcfc [out]

Type: <b><a href="https://msdn.microsoft.com/a5282277-85f5-494e-b994-efbf1116b519">NSTCFOLDERCAPABILITIES</a>*</b>

Pointer to a value that, when this method returns successfully, receives the capabilities requested in <i>nfcMask</i>. Except in the case of NSTCFC_NONE, bit values in positions not specifically requested in <i>nfcMask</i> do not necessarily reflect the capabilities and should not be used.



#### NSTCFC_NONE (0x00000000)

0x00000000. The <a href="https://msdn.microsoft.com/00937acb-1ce2-44f6-96a1-69e5dbb665f6">System.IsPinnedToNameSpaceTree</a> property does not exist on this folder. Filtering is not supported.



#### NSTCFC_PINNEDITEMFILTERING (0x00000001)

0x00000001. The <a href="https://msdn.microsoft.com/00937acb-1ce2-44f6-96a1-69e5dbb665f6">System.IsPinnedToNameSpaceTree</a> property exists on this folder and filtering based on that property value is supported.



#### NSTCFC_DELAY_REGISTER_NOTIFY (0x00000002)

0x00000002. Registration for change notifications is delayed until the folder is expanded in the navigation pane.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.


