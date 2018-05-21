---
UID: NF:cfgmgr32.CM_Enumerate_EnumeratorsW
title: CM_Enumerate_EnumeratorsW function
author: windows-driver-content
description: The CM_Enumerate_Enumerators function enumerates the local machine's device enumerators by supplying each enumerator's name.
old-location: devinst\cm_enumerate_enumerators.htm
old-project: devinst
ms.assetid: 85fbca44-bd3b-4654-bba2-099135c42d23
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Enumerate_Enumerators, CM_Enumerate_Enumerators function [Device and Driver Installation], CM_Enumerate_EnumeratorsW, cfgmgr32/CM_Enumerate_Enumerators, cfgmgr32/CM_Enumerate_EnumeratorsW, cfgmgrfn_16448772-e0d6-4182-9cfd-52bc354ce487.xml, devinst.cm_enumerate_enumerators
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: CM_Enumerate_EnumeratorsW (Unicode)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: CM_NOTIFY_ACTION, *PCM_NOTIFY_ACTION
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	LibDef
api_location:
-	Cfgmgr32.lib
-	Cfgmgr32.dll
api_name:
-	CM_Enumerate_Enumerators
-	CM_Enumerate_EnumeratorsW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Enumerate_EnumeratorsW function


## -description


The <b>CM_Enumerate_Enumerators</b> function enumerates the local machine's device enumerators by supplying each enumerator's name.


## -parameters




### -param ulEnumIndex [in]

Caller-supplied index into the machine's list of device enumerators. For more information, see the following <b>Remarks</b> section.


### -param Buffer [out]

Address of a buffer to receive an enumerator name. This buffer should be MAX_DEVICE_ID_LEN-sized (or, set <i>Buffer</i> to zero and obtain the actual name length in the location referenced by <i>puLength</i>).


### -param pulLength [in, out]

Caller-supplied address of a location to hold the buffer size. The caller supplies the length of the buffer pointed to by <i>Buffer</i>. The function replaces this value with the actual size of the enumerator's name string. If the caller-supplied buffer length is too small, the function supplies the required buffer size and returns CR_BUFFER_SMALL.


### -param ulFlags [in]

Not used, must be zero.


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



To enumerate the local machine's device enumerators, call <b>CM_Enumerate_Enumerators</b> repeatedly, starting with a <i>ulEnumIndex</i> index value of zero. and incrementing the index value with each subsequent call until the function returns CR_NO_SUCH_VALUE.

After enumerator names have been obtained, the names can be used as input to <a href="https://msdn.microsoft.com/library/windows/hardware/ff538415">CM_Get_Device_ID_List</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538032">CM_Enumerate_Enumerators_Ex</a>
 

 
