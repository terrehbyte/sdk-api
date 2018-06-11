---
UID: NF:sbtsv.ITsSbClientConnection.get_Environment
title: ITsSbClientConnection::get_Environment
author: windows-sdk-content
description: Retrieves an object that contains information about the environment that hosts the target computer.
old-location: termserv\itssbclientconnection_environment.htm
old-project: TermServ
ms.assetid: 97fe4851-96a9-4b23-8ad7-f42b87c655d0
ms.author: windowssdkdev
ms.date: 06/04/2018
ms.keywords: Environment property [Remote Desktop Services], Environment property [Remote Desktop Services],ITsSbClientConnection interface, ITsSbClientConnection interface [Remote Desktop Services],Environment property, ITsSbClientConnection.Environment, ITsSbClientConnection.get_Environment, ITsSbClientConnection::Environment, ITsSbClientConnection::get_Environment, get_Environment, sbtsv/ITsSbClientConnection::Environment, sbtsv/ITsSbClientConnection::get_Environment, termserv.itssbclientconnection_environment
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: sbtsv.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2012
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Sbtsv.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
tech.root: 
req.typenames: TS_SB_SORT_BY
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - sbtsv.h
api_name:
 - ITsSbClientConnection.Environment
 - ITsSbClientConnection.get_Environment
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# ITsSbClientConnection::get_Environment


## -description


Retrieves an object that contains information about the environment that hosts the target computer. For example, in a virtual desktop scenario, this object would contain information about the computer that hosts the virtual machine.

This property is read-only.


## -parameters


## -remarks



An orchestration plug-in can call this method to retrieve environment information about a target virtual machine.




## -see-also




<a href="https://msdn.microsoft.com/6649f43d-0e2a-42d7-8111-862bb28e3dbc">ITsSbClientConnection</a>
 

 
