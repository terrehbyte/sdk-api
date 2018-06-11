---
UID: NF:setupapi.SetupDiGetClassDevPropertySheetsA
title: SetupDiGetClassDevPropertySheetsA function
author: windows-sdk-content
description: The SetupDiGetClassDevPropertySheets function retrieves handles to the property sheets of a device information element or of the device setup class of a device information set.
old-location: devinst\setupdigetclassdevpropertysheets.htm
old-project: devinst
ms.assetid: cf5e8511-37be-4fb8-bded-b9b1e6bd247b
ms.author: windowssdkdev
ms.date: 05/31/2018
ms.keywords: SetupDiGetClassDevPropertySheets, SetupDiGetClassDevPropertySheets function [Device and Driver Installation], SetupDiGetClassDevPropertySheetsA, SetupDiGetClassDevPropertySheetsW, devinst.setupdigetclassdevpropertysheets, di-rtns_cdfb15cd-b7a4-42bf-ad4c-a3084a7a6d98.xml, setupapi/SetupDiGetClassDevPropertySheets
ms.prod: windows
ms.technology: windows-sdk
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
tech.root: 
req.typenames: TSSD_ConnectionPoint, *PTSSD_ConnectionPoint
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Setupapi.lib
 - Setupapi.dll
api_name:
 - SetupDiGetClassDevPropertySheets
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# SetupDiGetClassDevPropertySheetsA function


## -description


The <b>SetupDiGetClassDevPropertySheets</b> function retrieves handles to the property sheets of a device information element or of the <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a> of a device information set.


## -parameters




### -param DeviceInfoSet [in]

A handle to the <a href="devinst.device_information_sets">device information set</a> for which to return property sheet handles. If <i>DeviceInfoData</i> does not specify a device information element in the device information set, the device information set must have an associated device setup class. 


### -param DeviceInfoData [in, optional]

A pointer to an <a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a> structure that specifies a device information element in DeviceInfoSet. 

This parameter is optional and can be <b>NULL</b>. If this parameter is specified, <b>SetupDiGetClassDevPropertySheets</b> retrieves the property sheets handles that are associated with the specified device. If this parameter is <b>NULL</b>, <b>SetupDiGetClassDevPropertySheets</b> retrieves the property sheets handles that are associated with the device setup class specified in <i>DeviceInfoSet</i>.



### -param PropertySheetHeader [in]

A pointer to a PROPERTYSHEETHEADER structure. See the <b>Remarks</b> section for information about the caller-supplied array of property sheet handles that is associated with this structure. 

For more documentation on this structure and property sheets in general, see the Microsoft Windows SDK. 


### -param PropertySheetHeaderPageListSize [in]

The maximum number of handles that the caller-supplied array of property sheet handles can hold. 


### -param RequiredSize [out, optional]

A pointer to a variable of type DWORD that receives the number of property sheets that are associated with the specified device information element or the device setup class of the specified device information set. The pointer is optional and can be <b>NULL</b>. 


### -param PropertySheetType [in]

A flag that indicates one of the following types of property sheets.

<table>
<tr>
<th>Property sheet type</th>
<th>Meaning</th>
</tr>
<tr>
<td>
DIGCDP_FLAG_ADVANCED

</td>
<td>
Advanced property sheets.

</td>
</tr>
<tr>
<td>
DIGCDP_FLAG_BASIC

</td>
<td>
Basic property sheets. Supported only in Microsoft Windows 95 and Windows 98. Do not use in Windows 2000 and later versions of Windows.

</td>
</tr>
<tr>
<td>
DIGCDP_FLAG_REMOTE_ADVANCED

</td>
<td>
Advanced property sheets on a remote computer.

</td>
</tr>
</table>
 


## -returns



The function returns <b>TRUE</b> if successful. Otherwise, the function returns <b>FALSE</b>. Call <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a> to obtain the error code.




## -remarks



A PROPERTYSHEETHEADER structure contains two members that are associated with a caller-supplied array that the function uses to return the handles of property sheets. The <b>phpages</b> member is a pointer to a caller-supplied array of property sheet handles, and the input value of the <b>nPages</b> member specifies the number of handles that are already contained in the handle array. The function adds property sheet handles to the handle array beginning with the array element whose array index is the input value of <b>nPages</b>. The function adds handles to the array in consecutive order until either the array is full or the handles of all the requested property sheet pages have been added to the array. The maximum number of property sheet handles that the function can return is equal to (<i>PropertySheetHeaderPageListSize</i> - (input value of <b>nPages</b>)). 

If the handle array is large enough to hold the handles of all the requested property sheet pages, the function:

<ul>
<li>
Adds the handles to the handle array.

</li>
<li>
Sets <b>nPages</b> to the total number of handles in the array.

</li>
<li>
Sets <i>RequiredSize</i> to the number of handles that it returns.

</li>
<li>
Returns <b>TRUE</b>.

</li>
</ul>
If the handle array is not large enough to hold the handles of all the specified property sheet pages, the function: 

<ul>
<li>
Adds as many handles as the array can hold.

</li>
<li>
Sets <b>nPages</b> to <i>PropertySheetHeaderPageListSize</i>.

</li>
<li>
Sets <i>RequiredSize</i> to the total number of requested property sheet pages. The number of handles that are not returned by the function is equal to (<i>RequiredSize</i> - <i>PropertySheetHeaderPageListSize</i> - (input value of <b>nPages</b>)).

</li>
<li>
Sets the error code to ERROR_INSUFFICIENT_BUFFER.

</li>
<li>
Returns <b>FALSE</b>.

</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff552344">SP_DEVINFO_DATA</a>
 

 
