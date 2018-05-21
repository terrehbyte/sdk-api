---
UID: NF:shobjidl_core.IExplorerBrowser.BrowseToObject
title: IExplorerBrowser::BrowseToObject
author: windows-driver-content
description: Browses to an object.
old-location: shell\IExplorerBrowser_BrowseToObject.htm
old-project: shell
ms.assetid: cbfe2348-9fdc-4839-bf8b-b2a65caefa4c
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: BrowseToObject, BrowseToObject method [Windows Shell], BrowseToObject method [Windows Shell],IExplorerBrowser interface, IExplorerBrowser interface [Windows Shell],BrowseToObject method, IExplorerBrowser.BrowseToObject, IExplorerBrowser::BrowseToObject, SBSP_ABSOLUTE, SBSP_KEEPWORDWHEELTEXT, SBSP_NAVIGATEBACK, SBSP_NAVIGATEFORWARD, SBSP_PARENT, SBSP_RELATIVE, _shell_IExplorerBrowser_BrowseToObject, shell.IExplorerBrowser_BrowseToObject, shobjidl_core/IExplorerBrowser::BrowseToObject
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
-	IExplorerBrowser.BrowseToObject
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IExplorerBrowser::BrowseToObject


## -description


Browses to an object.


## -parameters




### -param punk [in]

Type: <b><a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a>*</b>

A pointer to an object to browse to. If the object cannot be browsed, an error value is returned.


### -param uFlags [in]

Type: <b>UINT</b>

A flag that specifies the category of the <i>pidl</i>. This affects how navigation is accomplished. Must be the value zero, or a bitwise combination of the following values.



#### SBSP_ABSOLUTE

An absolute PIDL, relative to the desktop.



#### SBSP_RELATIVE

A relative PIDL, relative to the current folder.



#### SBSP_PARENT

Browse the parent folder, ignore the PIDL.



#### SBSP_NAVIGATEBACK

Navigate back, ignore the PIDL.



#### SBSP_NAVIGATEFORWARD

Navigate forward, ignore the PIDL.





#### SBSP_KEEPWORDWHEELTEXT

<b>Windows Vista and later</b>. This flag indicates that any search text entered by a WordWheel (the Search box in Windows Explorer) should be preserved during this navigation, so that items at the new location are filtered in the same way they were filtered at the previous location.




## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



<i>uFlags</i> may be any of the <a href="https://msdn.microsoft.com/5be62600-147d-4625-8e6c-aa6687da2168">EXPLORER_BROWSER_FILL_FLAGS</a> or any of the flags defined in <a href="https://msdn.microsoft.com/e391ca11-25e3-4d97-8efd-0afd74a3e5c2">BrowseObject</a>'s <i>wFlags</i> parameter, except for flags that indicate navigation.

This method calls <a href="https://msdn.microsoft.com/2c05c2f5-5f72-436e-9b71-83749d3217b0">GetIDList</a> and browses to the pidl returned.  It operates in the same way as <a href="https://msdn.microsoft.com/b0633072-e059-4ea4-b9c0-798399ccf66a">IExplorerBrowser::BrowseToIDList</a>, except that <i>punk</i> cannot be <b>NULL</b>. Standard usage is to browse to an <a href="https://msdn.microsoft.com/35190a72-298b-4554-b924-e1357b583a99">IShellFolder</a> or an <a href="https://msdn.microsoft.com/599b9c0a-df04-4dbd-a5a6-a8736eecc560">IShellItem</a>. An error will be returned if the object passed in cannot be browsed through. An object that can be browsed through implements either <a href="https://msdn.microsoft.com/3deb3467-b6f2-49f9-ba24-fd2cca80f247">IPersistFolder2</a> or <a href="https://msdn.microsoft.com/b367dc07-8a50-4562-bd73-57c73c781d81">IPersistIDList</a>.

The first navigation of <a href="https://msdn.microsoft.com/da2cf5d4-5a68-4d18-807b-b9d4e2712c10">IExplorerBrowser</a> is synchronous. After that, all navigations are asynchronous. As a result, calls to <b>IExplorerBrowser::BrowseToObject</b> will succeed if you properly set up the pending   navigation, but that does not guarantee the navigation will succeed.  To be informed of success and failure, clients should implement <a href="https://msdn.microsoft.com/802d547f-41c2-4c4a-9f07-be615d7b86eb">IExplorerBrowserEvents</a> and respond appropriately in <a href="https://msdn.microsoft.com/54c97a55-a8d1-4635-a1e0-2f92d52ddc10">OnNavigationComplete</a> and <a href="https://msdn.microsoft.com/d4de3b81-4482-47c8-bb47-593aba484952">OnNavigationFailed</a>.


