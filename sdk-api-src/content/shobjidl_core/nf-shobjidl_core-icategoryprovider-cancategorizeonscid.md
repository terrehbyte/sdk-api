---
UID: NF:shobjidl_core.ICategoryProvider.CanCategorizeOnSCID
title: ICategoryProvider::CanCategorizeOnSCID
author: windows-driver-content
description: Determines whether a column can be used as a category.
old-location: shell\ICategoryProvider_CanCategorizeOnSCID.htm
old-project: shell
ms.assetid: e0b10007-7b25-4ddf-8cb9-76d85f8fb4df
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: CanCategorizeOnSCID, CanCategorizeOnSCID method [Windows Shell], CanCategorizeOnSCID method [Windows Shell],ICategoryProvider interface, ICategoryProvider interface [Windows Shell],CanCategorizeOnSCID method, ICategoryProvider.CanCategorizeOnSCID, ICategoryProvider::CanCategorizeOnSCID, inet_ICategoryProvider_CanCategorizeOnSCID, shell.ICategoryProvider_CanCategorizeOnSCID, shobjidl_core/ICategoryProvider::CanCategorizeOnSCID
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
-	Shell32.dll
api_name:
-	ICategoryProvider.CanCategorizeOnSCID
product: Windows
targetos: Windows
req.lib: 
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# ICategoryProvider::CanCategorizeOnSCID


## -description


Determines whether a column can be used as a category.


## -parameters




### -param pscid [in]

Type: <b>const <a href="https://msdn.microsoft.com/bf7b0e3b-527a-4ef5-894a-a7e1b7750e72">SHCOLUMNID</a>*</b>

A pointer to a <a href="https://msdn.microsoft.com/bf7b0e3b-527a-4ef5-894a-a7e1b7750e72">SHCOLUMNID</a> structure that identifies the column. Valid only when S_OK is returned. The GUID contained in this structure is then passed to <a href="https://msdn.microsoft.com/3703c061-4d21-4c36-900a-9ccacf4d482a">ICategoryProvider::CreateCategory</a>.


## -returns



Type: <b>HRESULT</b>

Returns S_OK if the column can be used as a category or S_FALSE if not.




## -remarks



When using the System Folder View Object in Category view (<b>Show in Groups</b>), the titles of columns for which this method returns S_OK appear in the upper portion of the <b>Arrange Icons By</b> submenu.


