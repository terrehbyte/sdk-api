---
UID: NF:setupapi.SetupDiBuildClassInfoList
title: SetupDiBuildClassInfoList function
author: windows-driver-content
description: The SetupDiBuildClassInfoList function returns a list of setup class GUIDs that identify the classes that are installed on a local computer.
old-location: devinst\setupdibuildclassinfolist.htm
old-project: devinst
ms.assetid: a01b1f8f-55af-4053-8c31-9329ef36f2ce
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiBuildClassInfoList, SetupDiBuildClassInfoList function [Device and Driver Installation], devinst.setupdibuildclassinfolist, di-rtns_25e014d5-5a99-42c3-8032-a24acd1856df.xml, setupapi/SetupDiBuildClassInfoList
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Microsoft Windows 2000 and later versions of Windows.
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
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Setupapi.dll
api_name:
-	SetupDiBuildClassInfoList
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiBuildClassInfoList function


## -description


The <b>SetupDiBuildClassInfoList</b> function returns a list of setup class GUIDs that identify the classes that are installed on a local computer.


## -parameters




### -param Flags [in]

Flags used to control exclusion of classes from the list. If no flags are specified, all setup classes are included in the list. Can be a combination of the following values:





#### DIBCI_NOINSTALLCLASS

Exclude a class if it has the <b>NoInstallClass</b> value entry in its registry key.



#### DIBCI_NODISPLAYCLASS

Exclude a class if it has the <b>NoDisplayClass</b> value entry in its registry key.


### -param ClassGuidList [out, optional]

A pointer to a GUID-typed array that receives a list of setup class GUIDs. This pointer is optional and can be <b>NULL</b>.


### -param ClassGuidListSize [in]

The number of GUIDs in the array that is pointed to by the <i>ClassGuildList</i> parameter. If <i>ClassGuidList</i> is <b>NULL</b>, <i>ClassGuidSize</i> must be zero.


### -param RequiredSize [out]

A pointer to a DWORD-typed variable that receives the number of GUIDs that are returned (if the number is less than or equal to the size, in GUIDs, of the array that is pointed to by the <i>ClassGuidList</i> parameter). 

If this number is greater than the size of the <i>ClassGuidList</i> array, it indicates how large the <i>ClassGuidList</i> array must be in order to contain all the class GUIDs.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved by making a call to <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -remarks



To retrieve the number of classes that are installed on a local computer, call <b>SetupDiBuildClassInfoList</b> with <i>ClassGuidList</i> set to <b>NULL</b> and <i>ClassGuidSize</i> set to zero. In response to such a call, the function returns the number of classes in <b>*</b><i>RequiredSize</i>.

<b>SetupDiBuildClassInfoList</b> does not return a class GUID for a class if the <b>NoUseClass</b> value entry exists in the registry key of the class.

To retrieve the list of setup class GUIDs installed on a remote system use <a href="https://msdn.microsoft.com/library/windows/hardware/ff550911">SetupDiBuildClassInfoListEx</a>. 




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff550911">SetupDiBuildClassInfoListEx</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551053">SetupDiGetClassDescription</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552010">SetupDiGetINFClass</a>
 

 
