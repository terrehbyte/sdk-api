---
UID: NE:vds._VDS_ISCSI_IPSEC_FLAG
title: "_VDS_ISCSI_IPSEC_FLAG"
author: windows-sdk-content
description: Not supported.This enumeration is reserved for future use.
old-location: base\vds_iscsi_ipsec_flag.htm
old-project: VDS
ms.assetid: e40789b4-ed34-4acc-8f69-5c3a93e44f82
ms.author: windowssdkdev
ms.date: 05/25/2018
ms.keywords: VDS_IIF_AGGRESSIVE_MODE, VDS_IIF_IKE, VDS_IIF_MAIN_MODE, VDS_IIF_PFS_ENABLE, VDS_IIF_TRANSPORT_MODE_PREFERRED, VDS_IIF_TUNNEL_MODE_PREFERRED, VDS_IIF_VALID, VDS_ISCSI_IPSEC_FLAG, VDS_ISCSI_IPSEC_FLAG enumeration [VDS], _VDS_ISCSI_IPSEC_FLAG, base.vds_iscsi_ipsec_flag, vds/VDS_IIF_AGGRESSIVE_MODE, vds/VDS_IIF_IKE, vds/VDS_IIF_MAIN_MODE, vds/VDS_IIF_PFS_ENABLE, vds/VDS_IIF_TRANSPORT_MODE_PREFERRED, vds/VDS_IIF_TUNNEL_MODE_PREFERRED, vds/VDS_IIF_VALID, vds/VDS_ISCSI_IPSEC_FLAG, vdshwprv/VDS_IIF_AGGRESSIVE_MODE, vdshwprv/VDS_IIF_IKE, vdshwprv/VDS_IIF_MAIN_MODE, vdshwprv/VDS_IIF_PFS_ENABLE, vdshwprv/VDS_IIF_TRANSPORT_MODE_PREFERRED, vdshwprv/VDS_IIF_TUNNEL_MODE_PREFERRED, vdshwprv/VDS_IIF_VALID, vdshwprv/VDS_ISCSI_IPSEC_FLAG
ms.prod: windows
ms.technology: windows-sdk
ms.topic: enum
req.header: vds.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.typenames: VDS_ISCSI_IPSEC_FLAG
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	Vds.h
-	VdsHwPrv.h
api_name:
-	VDS_ISCSI_IPSEC_FLAG
product: Windows
targetos: Windows
req.lib: VdmDbg.lib
req.dll: VdmDbg.dll
req.irql: 
req.product: Windows UI
---

# _VDS_ISCSI_IPSEC_FLAG enumeration


## -description


<p class="CCE_Message">[Beginning with Windows 8 and Windows Server 2012, the <a href="https://msdn.microsoft.com/536aafd2-cc04-48cc-8ee7-920efbba2a5f">Virtual Disk Service</a> COM interface is superseded by the <a href="https://msdn.microsoft.com/ff5e492d-5e62-4c9b-8f55-07859c9fee83">Windows Storage Management API</a>.]

Not supported.

This enumeration is reserved for future use.
   


## -enum-fields




### -field VDS_IIF_VALID

This bit must be set for the field to contain significant information.


### -field VDS_IIF_IKE

If set, IKE/IPSEC is enabled.


### -field VDS_IIF_MAIN_MODE

If set, negotiate through main mode is enabled.


### -field VDS_IIF_AGGRESSIVE_MODE

If set, negotiate through aggressive mode is enabled.


### -field VDS_IIF_PFS_ENABLE

If set, perfect forward secrecy is enabled.


### -field VDS_IIF_TRANSPORT_MODE_PREFERRED

If set, transport mode is preferred.


### -field VDS_IIF_TUNNEL_MODE_PREFERRED

If set, tunnel mode is preferred.


## -remarks



These flags are identical to the definitions for the iSNS portal security 
   bitmap.

<div class="alert"><b>Note</b>  Additional constants might be added to the <b>VDS_ISCSI_IPSEC_FLAG</b> enumeration in future Windows versions. For this reason, your application must be designed to gracefully handle an unrecognized <b>VDS_ISCSI_IPSEC_FLAG</b> enumeration constant.</div>
<div> </div>

