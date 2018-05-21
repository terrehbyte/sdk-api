---
UID: NF:shobjidl_core.ISearchFolderItemFactory.SetSortColumns
title: ISearchFolderItemFactory::SetSortColumns
author: windows-driver-content
description: Creates a list of sort column directions, as specified.
old-location: shell\ISearchFolderItemFactory_SetSortColumns.htm
old-project: shell
ms.assetid: c91667fa-a48b-409a-ba96-35581fdd07dd
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: ISearchFolderItemFactory interface [Windows Shell],SetSortColumns method, ISearchFolderItemFactory.SetSortColumns, ISearchFolderItemFactory::SetSortColumns, SetSortColumns, SetSortColumns method [Windows Shell], SetSortColumns method [Windows Shell],ISearchFolderItemFactory interface, _shell_ISearchFolderItemFactory_SetSortColumns, shell.ISearchFolderItemFactory_SetSortColumns, shobjidl_core/ISearchFolderItemFactory::SetSortColumns
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
-	ISearchFolderItemFactory.SetSortColumns
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# ISearchFolderItemFactory::SetSortColumns


## -description


Creates a list of sort column directions, as specified.


## -parameters




### -param cSortColumns [in]

Type: <b>UINT</b>

The number of sort columns.


### -param rgSortColumns [in]

Type: <b><a href="https://msdn.microsoft.com/3ca4c318-6462-4e22-813c-ef7b3ef03230">SORTCOLUMN</a>*</b>

A pointer to an array of <a href="https://msdn.microsoft.com/3ca4c318-6462-4e22-813c-ef7b3ef03230">SORTCOLUMN</a> structures containing sort direction.  The default is <b>PKEY_ItemNameDisplay</b>.


## -returns



Type: <b>HRESULT</b>

Returns a success value if successful, or an error value otherwise.


