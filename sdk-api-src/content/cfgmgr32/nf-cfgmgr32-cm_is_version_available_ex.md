---
UID: NF:cfgmgr32.CM_Is_Version_Available_Ex
title: CM_Is_Version_Available_Ex function
author: windows-driver-content
description: The CM_Is_Version_Available_Ex function indicates whether a specified version of the Plug and Play (PNP) Configuration Manager DLL (Cfgmgr32.dll) is supported by a local or a remote machine.
old-location: devinst\cm_is_version_available_ex.htm
old-project: devinst
ms.assetid: a6728f01-7899-46e3-8cda-19a5c46f4992
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Is_Version_Available_Ex, CM_Is_Version_Available_Ex function [Device and Driver Installation], cfgmgr32/CM_Is_Version_Available_Ex, cfgmgrfn_12196a98-8bca-4afa-8313-5a51f8c3cae1.xml, devinst.cm_is_version_available_ex
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows XP and later versions of Windows.
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
req.typenames: CM_NOTIFY_ACTION, *PCM_NOTIFY_ACTION
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Cfgmgr32.dll
api_name:
-	CM_Is_Version_Available_Ex
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: Cfgmgr32.dll
req.irql: 
---

# CM_Is_Version_Available_Ex function


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, this function has been deprecated and should not be used.]

The <b>CM_Is_Version_Available_Ex</b> function indicates whether a specified version of the Plug and Play (PNP) Configuration Manager <a href="https://msdn.microsoft.com/86688b5d-575d-42e1-9158-7ffba1aaf1d3">DLL</a> (<i>Cfgmgr32.dll</i>) is supported by a local or a remote machine.


## -parameters




### -param wVersion [in]

Identifies a version of the configuration manager. The supported version of the configuration manager corresponds directly to the operating system version. The major version is specified by the high-order byte and the minor version is specified by the low-order byte. For example, 0x0400 specifies version 4.0, which is supported by default by Microsoft Windows NT 4.0 and later versions of Windows. Version 0x0501 specifies version 5.1, which is supported by Windows XP and later versions of Windows. 


### -param hMachine [in, optional]

Supplies a machine handle that is returned by <a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>.

<div class="alert"><b>Note</b>  Using this function to access remote machines is not supported beginning with Windows 8 and Windows Server 2012, as this functionality has been removed.</div>
<div> </div>

## -returns



The function returns <b>TRUE</b> if the function can connect to the specified machine and if the machine supports the specified version. Otherwise, the function returns <b>FALSE</b>.




## -remarks



Use this function to determine whether a specified version of the configuration manager is supported by a local or a remote machine. If the specified version is supported, all versions earlier and including this version are supported by the machine. You can also use <a href="https://msdn.microsoft.com/library/windows/hardware/ff538736">CM_Is_Version_Available</a> to determine if the local machine supports a specific version of the configuration manager. 

 Functionality to access remote machines has been removed in Windows 8 and Windows Server 2012 and later operating systems thus you cannot access remote machines when running on these versions of Windows.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff537948">CM_Connect_Machine</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538686">CM_Get_Version</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538696">CM_Get_Version_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538736">CM_Is_Version_Available</a>
 

 
