---
UID: NF:xamlom.IVisualTreeServiceCallback2.OnElementStateChanged
title: IVisualTreeServiceCallback2::OnElementStateChanged
author: windows-sdk-content
description: Communicates the state of an element in the visual tree when it changes.
old-location: xaml_diagnostics\ivisualtreeservicecallback2_onelementstatechanged.htm
old-project: xaml_diagnostics
ms.assetid: A832FDC6-1485-432C-9A87-A3C94D0AF8CA
ms.author: windowssdkdev
ms.date: 06/04/2018
ms.keywords: IVisualTreeServiceCallback2 interface,OnElementStateChanged method, IVisualTreeServiceCallback2.OnElementStateChanged, IVisualTreeServiceCallback2::OnElementStateChanged, OnElementStateChanged, OnElementStateChanged method, OnElementStateChanged method,IVisualTreeServiceCallback2 interface, xaml_diagnostics.ivisualtreeservicecallback2_onelementstatechanged, xamlom/IVisualTreeServiceCallback2::OnElementStateChanged
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: xamlom.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: VisualMutationType
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - xamlom.h
api_name:
 - IVisualTreeServiceCallback2.OnElementStateChanged
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Use Windows Update or a Windows Update Services Server to retrieve the update on Windows XP.
---

# IVisualTreeServiceCallback2::OnElementStateChanged


## -description


Communicates the state of an element in the visual tree when it changes.


## -parameters




### -param element

The XAML element in the visual tree.


### -param elementState

The state of the element.


### -param context

The path to the element.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



When any XAML diagnostics API results in a resource reference becoming invalid, this callback will be notified of the invalid reference. An instance handle will be given that corresponds to an element in the tree, and a string representation of the path to the invalid reference. The grammar for the syntax is: PropertyName:Full.Dotted.TypeName[Indexer] and paths can be separated with a forward slash ("/") to be chained together. 




## -see-also




<a href="https://msdn.microsoft.com/F1C11F32-9524-49D6-89DD-C89E4A81720A">IVisualTreeServiceCallback2</a>
 

 
