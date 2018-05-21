---
UID: NE:cmdtree.DBVALUEKINDENUM
title: DBVALUEKINDENUM
author: windows-driver-content
description: The DBVALUEKINDENUM enumerated type is used to indicate the type of the union member inside a DBCOMMANDTREE structure.
old-location: indexsrv\dbvaluekindenum.htm
old-project: IndexSrv
ms.assetid: VS|indexsrv|~\html\ixoledb_8565.htm
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: DBVALUEKINDENUM, DBVALUEKINDENUM enumeration [Indexing Service], See below., _idxs_DBVALUEKINDENUM, cmdtree/DBVALUEKINDENUM, cmdtree/See below., indexsrv.dbvaluekindenum
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: cmdtree.h
req.include-header: 
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
req.typenames: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	cmdtree.h
api_name:
-	DBVALUEKINDENUM
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
---

# DBVALUEKINDENUM enumeration


## -description


<p class="CCE_Message">[Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use <a href="https://msdn.microsoft.com/6da601c6-3742-40ad-99f2-8817f7f642b3">Windows Search</a> for client side search and  <a href=" http://go.microsoft.com/fwlink/p/?linkid=258445">Microsoft Search Server Express</a> for server side search.]

The <b>DBVALUEKINDENUM</b> enumerated type is used to indicate the type of the union member inside a <a href="https://msdn.microsoft.com/141f1952-c1b7-4fbb-81d8-7ad3e9aa9b31">DBCOMMANDTREE</a> structure. For programming convenience, the values in this enumeration correspond exactly to the OLE Automation <b>VARENUM</b> and OLE DB <b>DBTYPE</b> enumerations. The comments associated with each enumeration value represent the type and branch of the union type inside the command structure containing the value. nodes that do not assign a value to the union member should assign a DBVALUEKIND_EMPTY to the <b>wKind</b> member of the <b>DBCOMMANDTREE</b> structure.


## -enum-fields




### -field DBVALUEKIND_BYGUID


### -field DBVALUEKIND_COLDESC


### -field DBVALUEKIND_ID


### -field DBVALUEKIND_CONTENT


### -field DBVALUEKIND_CONTENTVECTOR


### -field DBVALUEKIND_GROUPINFO


### -field DBVALUEKIND_PARAMETER


### -field DBVALUEKIND_PROPERTY


### -field DBVALUEKIND_SETFUNC


### -field DBVALUEKIND_SORTINFO


### -field DBVALUEKIND_TEXT


### -field DBVALUEKIND_COMMAND


### -field DBVALUEKIND_MONIKER


### -field DBVALUEKIND_ROWSET


### -field DBVALUEKIND_LIKE


### -field DBVALUEKIND_CONTENTPROXIMITY


### -field DBVALUEKIND_CONTENTSCOPE


### -field DBVALUEKIND_CONTENTTABLE


### -field DBVALUEKIND_IDISPATCH


### -field DBVALUEKIND_IUNKNOWN


### -field DBVALUEKIND_EMPTY


### -field DBVALUEKIND_NULL


### -field DBVALUEKIND_I2


### -field DBVALUEKIND_I4


### -field DBVALUEKIND_R4


### -field DBVALUEKIND_R8


### -field DBVALUEKIND_CY


### -field DBVALUEKIND_DATE


### -field DBVALUEKIND_BSTR


### -field DBVALUEKIND_ERROR


### -field DBVALUEKIND_BOOL


### -field DBVALUEKIND_VARIANT


### -field DBVALUEKIND_VECTOR


### -field DBVALUEKIND_ARRAY


### -field DBVALUEKIND_BYREF


### -field DBVALUEKIND_I1


### -field DBVALUEKIND_UI1


### -field DBVALUEKIND_UI2


### -field DBVALUEKIND_UI4


### -field DBVALUEKIND_I8


### -field DBVALUEKIND_UI8


### -field DBVALUEKIND_GUID


### -field DBVALUEKIND_BYTES


### -field DBVALUEKIND_STR


### -field DBVALUEKIND_WSTR


### -field DBVALUEKIND_NUMERIC


### -field DBVALUEKIND_DBDATE


### -field DBVALUEKIND_DBTIME


### -field DBVALUEKIND_DBTIMESTAMP


### -field DBVALUEKIND_PROBABILISTIC


### -field DBVALUEKIND_RELEVANTDOCUMENT




##### - See below.
