---
UID: NS:winnt._SYSTEM_ALARM_CALLBACK_ACE
title: "_SYSTEM_ALARM_CALLBACK_ACE"
author: windows-sdk-content
description: The SYSTEM_ALARM_CALLBACK_ACE structure is reserved for future use.
old-location: security\system_alarm_callback_ace.htm
old-project: SecAuthZ
ms.assetid: 8bfb579f-4bee-454e-827b-63a800bccf85
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: "*PSYSTEM_ALARM_CALLBACK_ACE, SYSTEM_ALARM_CALLBACK_ACE, SYSTEM_ALARM_CALLBACK_ACE structure [Security], _SYSTEM_ALARM_CALLBACK_ACE, security.system_alarm_callback_ace, winnt/SYSTEM_ALARM_CALLBACK_ACE"
ms.prod: windows
ms.technology: windows-sdk
ms.topic: struct
req.header: winnt.h
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
req.typenames: SYSTEM_ALARM_CALLBACK_ACE, *PSYSTEM_ALARM_CALLBACK_ACE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	Winnt.h
api_name:
-	SYSTEM_ALARM_CALLBACK_ACE
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Windows XP Professional x64 Edition or 64-bit editions of     Windows Server 2003
---

# _SYSTEM_ALARM_CALLBACK_ACE structure


## -description


Not supported.

The <b>SYSTEM_ALARM_CALLBACK_ACE</b> structure is reserved for future use.


## -struct-fields




### -field Header


<a href="https://msdn.microsoft.com/library/windows/hardware/ff538847">ACE_HEADER</a> structure that specifies the size and type of ACE. It also contains flags that control inheritance of the ACE by child objects. The <b>AceType</b> member of the <b>ACE_HEADER</b> structure should be set to SYSTEM_ALARM_CALLBACK_ACE_TYPE.


### -field Mask

Specifies an 
<a href="https://msdn.microsoft.com/library/windows/hardware/ff540466">ACCESS_MASK</a> structure that gives the access rights that cause audit messages to be generated. The SUCCESSFUL_ACCESS_ACE_FLAG and FAILED_ACCESS_ACE_FLAG flags in the <b>AceFlags</b> member of the <a href="https://msdn.microsoft.com/library/windows/hardware/ff538847">ACE_HEADER</a> structure indicate whether messages are generated for successful access attempts, unsuccessful access attempts, or both.


### -field SidStart

The first <b>DWORD</b> of a trustee's ACE. This ACE can be appended with application data. When the <a href="https://msdn.microsoft.com/e8a510e6-0739-4765-ad07-3bcb1b9c905c">AuthzAccessCheckCallback</a> function is called, this ACE is passed as the <i>pAce</i> parameter of that function.


## -remarks



ACE structures must be aligned on <b>DWORD</b> boundaries. All Windows memory-management functions return <b>DWORD</b>-aligned handles to memory.


