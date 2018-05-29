---
UID: NF:lmaccess.NetAccessEnum
title: NetAccessEnum function
author: windows-sdk-content
description: Not supported.
old-location: netmgmt\netaccessenum.htm
old-project: NetMgmt
ms.assetid: 34ffea84-ff41-43c3-864c-957178e9d22a
ms.author: windowssdkdev
ms.date: 05/22/2018
ms.keywords: 0, 1, NetAccessEnum, NetAccessEnum function [Network Management], _win32_netaccessenum, lmaccess/NetAccessEnum, netmgmt.netaccessenum
ms.prod: windows
ms.technology: windows-sdk
ms.topic: function
req.header: lmaccess.h
req.include-header: Lm.h, Lmaccess.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: MSA_INFO_STATE, *PMSA_INFO_STATE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Netapi32.dll
api_name:
-	NetAccessEnum
product: Windows
targetos: Windows
req.lib: Netapi32.lib
req.dll: Netapi32.dll
req.irql: 
req.product: GDI+ 1.1
---

# NetAccessEnum function


## -description


<p class="CCE_Message">[This function is obsolete. For a list of alternate functions, see <a href="https://msdn.microsoft.com/c236f335-b5de-4e8b-851d-45e008791271">Authorization Functions</a>.]

Not supported.

The <b>NetAccessEnum</b> function retrieves information about each access permission record.


## -parameters




### -param OPTIONAL

TBD




### -param BasePath

TBD


### -param Recursive

TBD


### -param level

TBD


### -param bufptr

TBD


### -param prefmaxlen

TBD


### -param entriesread

TBD


### -param totalentries

TBD


#### - cbBuffer

Specifies the size, in bytes, of the buffer pointed to by the <i>pbBuffer</i> parameter.


#### - fsRecursive

Specifies a flag that enables or disables recursive searching.
      

If this parameter is equal to zero, the <b>NetAccessEnum</b> function returns entries for the resource named as the base path by the <i>pszBasePath</i> parameter, and for the resources directly below that base path.

If this parameter is nonzero, the function returns entries for all access control lists (ACLs) that have <i>pszBasePath</i> at the beginning of the resource name.


#### - pbBuffer

Pointer to the buffer that receives the access information structure. The format of this data depends on the value of the <i>sLevel</i> parameter.


#### - pcEntriesRead

Pointer to an unsigned short integer that receives the count of elements actually enumerated. The count is valid only if the 
<b>NetAccessEnum</b> function returns <b>NERR_Success</b> or <b>ERROR_MORE_DATA</b>.


#### - pcTotalAvail

Pointer to an unsigned short integer that receives the total number of entries that could have been enumerated. The count is valid only if the 
<b>NetAccessEnum</b> function returns <b>NERR_Success</b> or <b>ERROR_MORE_DATA</b>.


#### - pszBasePath

Pointer to a string that contains a base pathname for the resource. A <b>NULL</b> pointer or <b>NULL</b> string means no base path is to be used. The path can be specified as a universal naming convention (UNC) pathname.


#### - pszServer

Pointer to a string that specifies the DNS or NetBIOS name of the remote server on which the function is to execute. If this parameter is <b>NULL</b>, the local computer is used.


#### - sLevel

Specifies the information level of the data. This parameter can be one of the following values.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="0"></a><dl>
<dt><b>0</b></dt>
</dl>
</td>
<td width="60%">
The <i>pbBuffer</i> parameter points to an 
<b>access_info_0</b> structure.

</td>
</tr>
<tr>
<td width="40%"><a id="1"></a><dl>
<dt><b>1</b></dt>
</dl>
</td>
<td width="60%">
The <i>pbBuffer</i> parameter points to an 
<b>access_info_1</b> structure.

</td>
</tr>
</table>
 


## -returns



If the function succeeds, the return value is <b>NERR_Success</b>.

If the function fails, the return value is a system error code. For a list of error codes, see 
<a href="https://msdn.microsoft.com/4a3a8feb-a05f-4614-8f04-1f507da7e5b7">System Error Codes</a>.




## -remarks



This function requires Admin privilege to successfully execute on a computer that has local security enabled.




## -see-also




<a href="https://msdn.microsoft.com/c236f335-b5de-4e8b-851d-45e008791271">Authorization Functions</a>
 

 
