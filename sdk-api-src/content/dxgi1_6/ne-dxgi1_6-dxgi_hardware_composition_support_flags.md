---
UID: NE:dxgi1_6.DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS
title: DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS
author: windows-driver-content
description: Describes which levels of hardware composition are supported.
old-location: direct3ddxgi\dxgi_hardware_composition_support_flags.htm
old-project: direct3ddxgi
ms.assetid: FA8BCF74-58CB-4806-A0A5-1D8E6EC576DC
ms.author: windowsdriverdev
ms.date: 5/17/2018
ms.keywords: DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS, DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS enumeration [DXGI], DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_CURSOR_STRETCHED, DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_FULLSCREEN, DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_WINDOWED, direct3ddxgi.dxgi_hardware_composition_support_flags, dxgi1_6/DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS, dxgi1_6/DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_CURSOR_STRETCHED, dxgi1_6/DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_FULLSCREEN, dxgi1_6/DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_WINDOWED
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: dxgi1_6.h
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
req.typenames: DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	dxgi1_6.h
api_name:
-	DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows Media Format 9 Series or later
---

# DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS enumeration


## -description


Describes which levels of hardware composition are supported.


## -enum-fields




### -field DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_FULLSCREEN

This flag specifies that swapchain composition can be facilitated in a performant manner using hardware for fullscreen applications.


### -field DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_WINDOWED

This flag specifies that swapchain composition can be facilitated in a performant manner using hardware for windowed applications.


### -field DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAG_CURSOR_STRETCHED

This flag specifies that swapchain composition facilitated using hardware can cause the cursor to appear stretched.


## -remarks



Values of this enumeration are returned from the <a href="direct3ddxgi.idxgioutput6_checkhardwarecompositionsupport">IDXGIOutput6::CheckHardwareCompositionSupport</a> method in the <i>pFlags</i> out parameter.




## -see-also




<a href="https://msdn.microsoft.com/c4574c89-dee2-4841-9318-5383cf417111">DXGI Enumerations</a>



<a href="direct3ddxgi.idxgioutput6_checkhardwarecompositionsupport">IDXGIOutput6::CheckHardwareCompositionSupport method</a>
 

 
