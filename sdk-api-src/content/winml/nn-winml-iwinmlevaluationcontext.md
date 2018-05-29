---
UID: NN:winml.IWinMLEvaluationContext
title: IWinMLEvaluationContext
author: windows-sdk-content
description: Represents the context to bind inputs and outputs to a WinML model.
old-location: machinelearning\iwinmlevaluationcontext.htm
old-project: MachineLearning
ms.assetid: D4C9B16A-B351-41E4-AD42-20C25F3CC404
ms.author: windowssdkdev
ms.date: 03/07/2018
ms.keywords: IWinMLEvaluationContext, IWinMLEvaluationContext interface, IWinMLEvaluationContext interface,described, MachineLearning.iwinmlevaluationcontext, winml/IWinMLEvaluationContext
ms.prod: windows
ms.technology: windows-sdk
ms.topic: interface
req.header: winml.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10, version 1803 [desktop apps only]
req.target-min-winversvr: Windows Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: WINML_TENSOR_DATA_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	winml.dll
api_name:
-	IWinMLEvaluationContext
product: Windows
targetos: Windows
req.lib: Winml.lib
req.dll: Winml.dll
req.irql: 
req.product: Windows Address Book 5.0
---

# IWinMLEvaluationContext interface


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Represents the context to bind inputs and outputs to a WinML model.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWinMLEvaluationContext</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWinMLEvaluationContext</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWinMLEvaluationContext</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/3D417952-92DD-4111-9060-C7F8CCA456AB">BindValue </a>
</td>
<td align="left" width="63%">
Binds the input/output to the given model.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/hh406339">Clear</a>
</td>
<td align="left" width="63%">
Clears the bindings for a model.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/750A799F-A5A7-48D2-958B-D03423C0CE09">GetValueByName</a>
</td>
<td align="left" width="63%">
Returns the input/output description for the specific binding name.

</td>
</tr>
</table> 
