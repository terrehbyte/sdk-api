---
UID: NF:winml.IWinMLRuntime.EvaluateModel
title: IWinMLRuntime::EvaluateModel
author: windows-sdk-content
description: Evaluates a WinML model.
old-location: machinelearning\iwinmlruntime_evaluatemodel.htm
old-project: MachineLearning
ms.assetid: F96A1CCD-02BD-4E93-830D-9975A03658E2
ms.author: windowssdkdev
ms.date: 03/07/2018
ms.keywords: EvaluateModel, EvaluateModel method, EvaluateModel method,IWinMLRuntime interface, IWinMLRuntime interface,EvaluateModel method, IWinMLRuntime.EvaluateModel, IWinMLRuntime::EvaluateModel, MachineLearning.iwinmlruntime_evaluatemodel, winml/IWinMLRuntime::EvaluateModel
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
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
-	IWinMLRuntime.EvaluateModel
product: Windows
targetos: Windows
req.lib: Winml.lib
req.dll: Winml.dll
req.irql: 
req.product: Windows Address Book 5.0
---

# IWinMLRuntime::EvaluateModel


## -description


<p class="CCE_Message">[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.]

Evaluates a WinML model.


## -parameters




### -param pContext [in]

A pointer to the <a href="https://msdn.microsoft.com/D4C9B16A-B351-41E4-AD42-20C25F3CC404">WinMLEvaluationContext</a> to evaluate.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/C2FD74A1-EE38-46B1-98A8-43557485F92E">IWinMLRuntime</a>
 

 
