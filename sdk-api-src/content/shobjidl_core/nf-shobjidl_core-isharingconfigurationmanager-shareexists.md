---
UID: NF:shobjidl_core.ISharingConfigurationManager.ShareExists
title: ISharingConfigurationManager::ShareExists
author: windows-driver-content
description: Queries whether the Users or Public folder is shared.
old-location: shell\ISharingConfigurationManager_ShareExists.htm
old-project: shell
ms.assetid: d15d40a1-fdde-430a-bb8c-537ce58536dd
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ISharingConfigurationManager interface [Windows Shell],ShareExists method, ISharingConfigurationManager.ShareExists, ISharingConfigurationManager::ShareExists, ShareExists, ShareExists method [Windows Shell], ShareExists method [Windows Shell],ISharingConfigurationManager interface, _shell_ISharingConfigurationManager_ShareExists, shell.ISharingConfigurationManager_ShareExists, shobjidl_core/ISharingConfigurationManager::ShareExists
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
-	ISharingConfigurationManager.ShareExists
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ISharingConfigurationManager::ShareExists


## -description


Queries whether the <b>Users</b> or <b>Public</b> folder is shared.


## -parameters




### -param dsid [in]

Type: <b><a href="https://msdn.microsoft.com/02d3b664-eeef-4214-99e8-246241103c4e">DEF_SHARE_ID</a></b>

One of the <a href="https://msdn.microsoft.com/02d3b664-eeef-4214-99e8-246241103c4e">DEF_SHARE_ID</a> values that indicates the folder whose sharing state is being checked.


## -returns



Type: <b>HRESULT</b>

S_OK if the folder is shared; otherwise, S_FALSE.




## -remarks



Because as of Windows 7 <b>Public</b> is shared in-place through <b>Users</b>, callers should always check for the Users share first. If a share is found to exist on <b>Users</b>, then it follows that a share exists on <b>Public</b> as well.


