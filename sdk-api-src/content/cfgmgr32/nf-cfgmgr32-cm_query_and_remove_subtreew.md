---
UID: NF:cfgmgr32.CM_Query_And_Remove_SubTreeW
title: CM_Query_And_Remove_SubTreeW function
author: windows-driver-content
description: The CM_Query_And_Remove_SubTree function checks whether a device instance and its children can be removed and, if so, it removes them.
old-location: devinst\cm_query_and_remove_subtree.htm
old-project: devinst
ms.assetid: 0a80cddd-d5be-42cb-ba11-0a3292b973a3
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: CM_Query_And_Remove_SubTree, CM_Query_And_Remove_SubTree function [Device and Driver Installation], CM_Query_And_Remove_SubTreeW, cfgmgr32/CM_Query_And_Remove_SubTree, cfgmgr32/CM_Query_And_Remove_SubTreeW, cfgmgrfn_81d4975f-cc31-49aa-8fa7-984abd25c26b.xml, devinst.cm_query_and_remove_subtree
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: cfgmgr32.h
req.include-header: Cfgmgr32.h
req.target-type: Universal
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: CM_Query_And_Remove_SubTreeW (Unicode)
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
-	Cfgmgr32.lib
-	Cfgmgr32.dll
-	API-Ms-Win-Devices-Config-L1-1-0.dll
-	API-Ms-Win-Devices-Config-L1-1-1.dll
-	CfgMgr32.dll
api_name:
-	CM_Query_And_Remove_SubTree
-	CM_Query_And_Remove_SubTreeW
product: Windows
targetos: Windows
req.lib: Cfgmgr32.lib
req.dll: 
req.irql: 
---

# CM_Query_And_Remove_SubTreeW function


## -description


The <b>CM_Query_And_Remove_SubTree</b> function checks whether a device instance and its children can be removed and, if so, it removes them.


## -parameters




### -param dnAncestor [in]

Caller-supplied device instance handle to the device at the root of the subtree to be removed. This device instance handle is bound to the local machine. 


### -param pVetoType [out, optional]

(<i>Optional</i>) If not <b>NULL</b>, this points to a location that, if the removal request fails, receives a <a href="https://msdn.microsoft.com/library/windows/hardware/ff549728">PNP_VETO_TYPE</a>-typed value indicating the reason for the failure.


### -param pszVetoName [out, optional]

(<i>Optional</i>) If not <b>NULL</b>, this is a caller-supplied pointer to a string buffer that receives a text string. The type of information this string provides is dependent on the value received by <i>pVetoType</i>. For information about these strings, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff549728">PNP_VETO_TYPE</a>.


### -param ulNameLength [in]

Caller-supplied value representing the length (number of characters) of the string buffer supplied by <i>pszVetoName</i>. This should be set to MAX_PATH.


### -param ulFlags [in]

A bitwise OR of the caller-supplied flag constants that are described in the <b>Remarks</b> section. 


## -returns



If the operation succeeds, the function returns CR_SUCCESS. Otherwise, it returns one of the CR_-prefixed error codes defined in <i>Cfgmgr32.h</i>.




## -remarks



The purpose of the <b>CM_Query_And_Remove_SubTree</b> function is to allow an application to prepare a device for safe removal from the local machine. Use this function to remove devices only if a driver has not set the <b>SurpriseRemovalOK</b> member of <a href="https://msdn.microsoft.com/library/windows/hardware/ff543095">DEVICE_CAPABILITIES</a>. If a driver has set <b>SurpriseRemovalOK</b>, the application should call <a href="https://msdn.microsoft.com/library/windows/hardware/ff539806">CM_Request_Device_Eject</a> instead of <b>CM_Query_And_Remove_SubTree</b>.

<b>CM_Query_And_Remove_SubTree</b> supports setting the flags parameter <i>ulFlags</i> with one of the following two flags; these flags apply only if Windows or an installer vetoes the removal of a device: 



Beginning with Windows XP, <b>CM_Query_And_Remove_SubTree</b> also supports setting the following additional flag; this flag applies only if the function successfully removes the device instance:



Windows applications that do not require the low-level operation <b>CM_Query_And_Remove_SubTree</b> should use the <a href="https://msdn.microsoft.com/library/windows/hardware/ff543712">DIF_PROPERTYCHANGE</a> request to disable a device instead of using <b>CM_Query_And_Remove_SubTree</b> to remove a device. The DIF_PROPERTYCHANGE request can be used to enable, disable, restart, stop, or change the properties of a device. 

Callers of this function must have <b>SeLoadDriverPrivilege</b>. (Privileges are described in the Microsoft Windows SDK documentation.)

For information about using device instance handles that are bound to the local machine, see <a href="https://msdn.microsoft.com/library/windows/hardware/ff538074">CM_Get_Child</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff538074">CM_Get_Child</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff539727">CM_Query_And_Remove_SubTree_Ex</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff539763">CM_Reenumerate_DevNode</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff539806">CM_Request_Device_Eject</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff539825">CM_Setup_DevNode</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543712">DIF_PROPERTYCHANGE</a>
 

 
