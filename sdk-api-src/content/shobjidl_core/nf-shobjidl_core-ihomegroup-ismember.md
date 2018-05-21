---
UID: NF:shobjidl_core.IHomeGroup.IsMember
title: IHomeGroup::IsMember
author: windows-driver-content
description: Determines whether the local computer is a member of a HomeGroup.
old-location: shell\IHomeGroup_IsMember.htm
old-project: shell
ms.assetid: 9ce98b11-46fd-4168-828d-a5ba8f71b7c9
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IHomeGroup interface [Windows Shell],IsMember method, IHomeGroup.IsMember, IHomeGroup::IsMember, IsMember, IsMember method [Windows Shell], IsMember method [Windows Shell],IHomeGroup interface, _shell_IHomeGroup_IsMember, shell.IHomeGroup_IsMember, shobjidl_core/IHomeGroup::IsMember
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
-	IHomeGroup.IsMember
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IHomeGroup::IsMember


## -description


Determines whether the local computer is a member of a HomeGroup.


## -parameters




### -param member [out]

Type: <b>BOOL*</b>

When this method returns successfully, receives <b>TRUE</b> if the local computer is a member of a HomeGroup; otherwise, <b>FALSE</b>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The following code snippet shows how to create an instance of <a href="https://msdn.microsoft.com/97d693c0-1126-4cd3-8aee-b5499b538403">IHomeGroup</a> and call <b>IHomeGroup::IsMember</b>.
         
                

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>#include "shobjidl.h"
#include "atlbase.h"   // For COM smart pointers
                    
CComPtr&lt;IHomeGroup&gt; spHomeGroup;
HRESULT hr = S_OK;
BOOL fIsHGMember = FALSE;

// Initialize the COM subsystem.
hr = CoInitialize(NULL);
if (FAILED(hr)) return hr;

// Create an instance of IHomeGroup.
hr = CoCreateInstance(CLSID_HomeGroup, 
                      NULL, 
                      CLSCTX_INPROC_SERVER, 
                      IID_PPV_ARGS(&amp;spHomeGroup));

if (FAILED(hr)) return hr;

// fIsHGMember receives the value TRUE if the local computer is a member of a 
// HomeGroup, or FALSE if the computer is not a HomeGroup member.
hr = spHomeGroup-&gt;IsMember(&amp;fIsHGMember);</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="22d9ea8d-ed66-4c34-940f-141db11e83bd">CComPtr</a>



<a href="https://msdn.microsoft.com/7295a55b-12c7-4ed0-a7a4-9ecee16afdec">CoCreateInstance</a>



<a href="https://msdn.microsoft.com/0f171cf4-87b9-43a6-97f2-80ed344fe376">CoInitialize</a>



<a href="https://msdn.microsoft.com/97d693c0-1126-4cd3-8aee-b5499b538403">IHomeGroup</a>
 

 
