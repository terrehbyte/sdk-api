---
UID: NN:shobjidl_core.IObjectProvider
title: IObjectProvider
author: windows-driver-content
description: Exposes a method to discover objects that are named with a GUID from another object. Unlike QueryService this interface will not delegate its functionality on to other objects.
old-location: shell\IObjectProvider.htm
old-project: shell
ms.assetid: 477991e5-0882-475c-9178-c3add695dc2c
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IObjectProvider, IObjectProvider interface [Windows Shell], IObjectProvider interface [Windows Shell],described, _shell_IObjectProvider, shell.IObjectProvider, shobjidl_core/IObjectProvider
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
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
-	IObjectProvider
product: Windows
targetos: Windows
req.lib: Shell32.lib
req.dll: Shell32.dll
req.irql: 
req.product: Outlook Express 6.0
---

# IObjectProvider interface


## -description


Exposes a method to discover objects that are named with a <b>GUID</b> from another object. Unlike <a href="_inet_IServiceProvider_QueryService_Method">QueryService</a> this interface will not delegate its functionality on to other objects.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IObjectProvider</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IObjectProvider</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IObjectProvider</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7bd76e54-bc1d-481d-90cb-fcfe519b8bfb">QueryObject</a>
</td>
<td align="left" width="63%">
Queries for a specified object.

</td>
</tr>
</table> 


## -remarks



Similar to <a href="_inet_IServiceProvider_Interface">IServiceProvider</a>, except that this method does not imply that unhandled or unknown requests should be forwarded.


