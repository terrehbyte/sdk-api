---
UID: NE:shobjidl_core._KF_REDIRECT_FLAGS
title: "_KF_REDIRECT_FLAGS"
author: windows-driver-content
description: Flags used by IKnownFolderManager::Redirect to specify details of a known folder redirection such as permissions and ownership for the redirected folder.
old-location: shell\KF_REDIRECT_FLAGS.htm
old-project: shell
ms.assetid: 6016f02f-5480-4fd8-b21d-209ebd863922
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: KF_REDIRECT_CHECK_ONLY, KF_REDIRECT_COPY_CONTENTS, KF_REDIRECT_COPY_SOURCE_DACL, KF_REDIRECT_DEL_SOURCE_CONTENTS, KF_REDIRECT_EXCLUDE_ALL_KNOWN_SUBFOLDERS, KF_REDIRECT_FLAGS, KF_REDIRECT_FLAGS enumeration [Windows Shell], KF_REDIRECT_OWNER_USER, KF_REDIRECT_PIN, KF_REDIRECT_SET_OWNER_EXPLICIT, KF_REDIRECT_UNPIN, KF_REDIRECT_USER_EXCLUSIVE, KF_REDIRECT_WITH_UI, _KF_REDIRECT_FLAGS, _shell_KF_REDIRECT_FLAGS, shell.KF_REDIRECT_FLAGS, shobjidl_core/KF_REDIRECT_CHECK_ONLY, shobjidl_core/KF_REDIRECT_COPY_CONTENTS, shobjidl_core/KF_REDIRECT_COPY_SOURCE_DACL, shobjidl_core/KF_REDIRECT_DEL_SOURCE_CONTENTS, shobjidl_core/KF_REDIRECT_EXCLUDE_ALL_KNOWN_SUBFOLDERS, shobjidl_core/KF_REDIRECT_FLAGS, shobjidl_core/KF_REDIRECT_OWNER_USER, shobjidl_core/KF_REDIRECT_PIN, shobjidl_core/KF_REDIRECT_SET_OWNER_EXPLICIT, shobjidl_core/KF_REDIRECT_UNPIN, shobjidl_core/KF_REDIRECT_USER_EXCLUSIVE, shobjidl_core/KF_REDIRECT_WITH_UI
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
-	shobjidl_core.h
api_name:
-	KF_REDIRECT_FLAGS
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Internet Explorer 6.01
---

# _KF_REDIRECT_FLAGS enumeration


## -description


Flags used by <a href="https://msdn.microsoft.com/0f4fc609-597b-4c72-b875-4b3f051dd056">IKnownFolderManager::Redirect</a> to specify details of a known folder redirection such as permissions and ownership for the redirected folder.


## -enum-fields




### -field KF_REDIRECT_USER_EXCLUSIVE

Ensure that only the user has permission to access the redirected folder.


### -field KF_REDIRECT_COPY_SOURCE_DACL

Copy the DACL of the source folder to the target to maintain current access permissions.


### -field KF_REDIRECT_OWNER_USER

Sets the user as the owner of a newly created target folder unless the user is a member of the Administrator group, in which case Administrator is set as the owner. Must be called with KF_REDIRECT_SET_OWNER_EXPLICIT.


### -field KF_REDIRECT_SET_OWNER_EXPLICIT

Set the owner of a newly created target folder.  If the user belongs to the Administrators group, Administrators is assigned as the owner. Must be called with KF_REDIRECT_OWNER_USER.


### -field KF_REDIRECT_CHECK_ONLY

Do not perform a redirection, simply check whether redirection has occurred. If so, <a href="https://msdn.microsoft.com/0f4fc609-597b-4c72-b875-4b3f051dd056">IKnownFolderManager::Redirect</a> returns S_OK; if not, or if some actions remain to be completed, it returns S_FALSE.


### -field KF_REDIRECT_WITH_UI

Display UI during the redirection.


### -field KF_REDIRECT_UNPIN

Unpin the source folder.


### -field KF_REDIRECT_PIN

Pin the target folder.


### -field KF_REDIRECT_COPY_CONTENTS

Copy the existing contents—both files and subfolders—of the known folder to the redirected folder.


### -field KF_REDIRECT_DEL_SOURCE_CONTENTS

Delete the contents of the source folder after they have been copied to the redirected folder. This flag is valid only if <a href="https://msdn.microsoft.com/6016f02f-5480-4fd8-b21d-209ebd863922">KF_REDIRECT_COPY_CONTENTS</a> is set.


### -field KF_REDIRECT_EXCLUDE_ALL_KNOWN_SUBFOLDERS

Reserved. Do not use.


## -remarks



The <b><b>KF_REDIRECT_OWNER_USER</b></b> and <b><b>KF_REDIRECT_SET_OWNER_EXPLICIT</b></b> flags provide ownership checks for the target folder, if that folder exists. By default, <a href="https://msdn.microsoft.com/0f4fc609-597b-4c72-b875-4b3f051dd056">IKnownFolderManager::Redirect</a> does not perform ownership checks. KF_REDIRECT_OWNER_USER and KF_REDIRECT_SET_OWNER_EXPLICIT are only valid if called together.

The <b>KF_REDIRECT_FLAGS</b> type is defined in Shobjidl.h as shown here.

<div class="code"><span codelanguage=""><table>
<tr>
<th></th>
</tr>
<tr>
<td>
<pre>typedef DWORD KF_REDIRECT_FLAGS;</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/49799A9E-BA86-4977-B5F3-590BE1E5FBF6">Known Folders Sample</a>
 

 
