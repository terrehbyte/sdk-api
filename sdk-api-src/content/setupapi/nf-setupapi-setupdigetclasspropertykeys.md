---
UID: NF:setupapi.SetupDiGetClassPropertyKeys
title: SetupDiGetClassPropertyKeys function
author: windows-driver-content
description: The SetupDiGetClassPropertyKeys function retrieves an array of the device property keys that represent the device properties that are set for a device setup class or a device interface class.
old-location: devinst\setupdigetclasspropertykeys.htm
old-project: devinst
ms.assetid: 9b595fc5-f517-41f9-b7a8-a7811f658d57
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: SetupDiGetClassPropertyKeys, SetupDiGetClassPropertyKeys function [Device and Driver Installation], devinst.setupdigetclasspropertykeys, di-rtns_7f87ef8b-8752-4cd4-9aca-811a83c99ccf.xml, setupapi/SetupDiGetClassPropertyKeys
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: DesktopFor universal, call CM_Get_Class_Property_Keys
req.target-min-winverclnt: Available in Windows Vista and later versions of Windows.
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
-	SetupDiGetClassPropertyKeys
product: Windows
targetos: Windows
req.lib: Setupapi.lib
req.dll: Setupapi.dll
req.irql: 
req.product: Rights Management Services client 1.0 SP2 or later
---

# SetupDiGetClassPropertyKeys function


## -description


The <b>SetupDiGetClassPropertyKeys</b> function retrieves an array of the device property keys that represent the device properties that are set for a <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff552344">device setup class</a> or a <a href="https://msdn.microsoft.com/C989D2D3-E8DE-4D64-86EE-3D3B3906390D">device interface class</a>.


## -parameters




### -param ClassGuid [in]

A pointer to a GUID that represents a device setup class or a device interface class. <b>SetupDiGetClassPropertyKeys</b> retrieves an array of the device property keys that represent device properties that are set for the specified class. For information about specifying the class type, see the <i>Flags</i> parameter.


### -param PropertyKeyArray [out, optional]

A pointer to a buffer that receives an array of <a href="https://msdn.microsoft.com/library/windows/hardware/dn315031">DEVPROPKEY</a>-typed values, where each value is a device property key that represents a device property that is set for the device class. The pointer is optional and can be <b>NULL</b>. For more information, see the <b>Remarks</b> section later in this topic.


### -param PropertyKeyCount [in]

The size, in DEVPROPKEY-typed values, of the <i>PropertyKeyArray</i> buffer. If <i>PropertyKeyArray</i> is set to <b>NULL</b>, <i>PropertyKeyCount</i> must be set to zero.


### -param RequiredPropertyKeyCount [out, optional]

A pointer to a DWORD-typed variable that receives the number of requested property keys. The parameter is optional and can be set to <b>NULL</b>. 


### -param Flags [in]

One of the following values, which specifies whether to retrieve property keys for a device setup class or for a device interface class:





#### DICLASSPROP_INSTALLER

<i>ClassGuid</i> specifies a device setup class. This flag cannot be used with DICLASSPROP_INTERFACE.



#### DICLASSPROP_INTERFACE

<i>ClassGuid</i> specifies a device interface class. This flag cannot be used with DICLASSPROP_INSTALLER.


## -returns



<b>SetupDiGetClassPropertyKeys</b> returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b>, and the logged error can be retrieved by calling <a href="http://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.

The following table includes some of the more common error codes that this function might log.


<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_FLAGS</b></dt>
</dl>
</td>
<td width="60%">
The value of<i> Flags</i> is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_CLASS</b></dt>
</dl>
</td>
<td width="60%">
If the DICLASSPROP_INSTALLER flag is specified, this error code indicates that the device setup class that is specified by <i>ClassGuid</i> does not exist. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_REFERENCE_STRING</b></dt>
</dl>
</td>
<td width="60%">
The reference string for the device interface that is specified by <i>ClassGuild</i> is not valid. This error can be returned if the DICLASSPROP_INTERFACE flag is specified. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_DATA</b></dt>
</dl>
</td>
<td width="60%">
An unspecified data value is not valid. One possibility is that the <i>ClassGuid</i> value is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
An unspecified parameter is not valid. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INVALID_USER_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
A user buffer is not valid. One possibility is that <i>PropertyKeyArray</i> is <b>NULL</b>, and <i>PropertKeyCount</i> is not zero.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NO_SUCH_INTERFACE_CLASS</b></dt>
</dl>
</td>
<td width="60%">
If the DICLASSPROP_INTERFACE flag is specified, this error code indicates that the device interface class that is specified by <i>ClassGuid</i> does not exist. 

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_INSUFFICENT_BUFFER</b></dt>
</dl>
</td>
<td width="60%">
The <i>PropertyKeyArray</i> buffer is not large enough to hold all the property keys, or an internal data buffer that was passed to a system call was too small.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_NOT_ENOUGH_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
There was not enough system memory available to complete the operation.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have Administrator privileges. 

</td>
</tr>
</table>
 




## -remarks



<b>SetupDiGetClassPropertyKeys</b> is part of the <a href="devinst.unified_device_property_model__windows_vista_and_later_">unified device property model</a>. 

A caller of <b>SetupDiGetClassPropertyKeys</b> must be a member of the Administrators group to retrieve device property keys for a device class. 

If the <i>PropertyKeyArray</i> buffer is not large enough to hold all the requested property keys, <b>SetupDiGetClassPropertyKeys</b> does not retrieve any property keys and returns ERROR_INSUFFICIENT_BUFFER. If the caller supplied a <i>RequiredPropertyKeyCount</i> pointer, <b>SetupDiGetClassPropertyKeys</b> sets the value of *<i>RequiredPropertyKeyCount</i> to the required size, in DEVPROPKEY-typed values, of the <i>PropertyKeyArray </i>buffer<i>.</i>

To retrieve a device class property on a local computer, call <a href="https://msdn.microsoft.com/library/windows/hardware/ff551086">SetupDiGetClassProperty</a>. To set a device class property on a local computer, call <a href="https://msdn.microsoft.com/library/windows/hardware/ff552128">SetupDiSetClassProperty</a>.

To retrieve the property keys for a device setup class or device interface class on a remote computer, call <a href="https://msdn.microsoft.com/library/windows/hardware/ff551093">SetupDiGetClassPropertyKeysEx</a>.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff551086">SetupDiGetClassProperty</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff551093">SetupDiGetClassPropertyKeysEx</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff552128">SetupDiSetClassProperty</a>
 

 
