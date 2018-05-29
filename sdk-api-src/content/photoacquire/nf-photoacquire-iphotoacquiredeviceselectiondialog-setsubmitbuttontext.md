---
UID: NF:photoacquire.IPhotoAcquireDeviceSelectionDialog.SetSubmitButtonText
title: IPhotoAcquireDeviceSelectionDialog::SetSubmitButtonText
author: windows-sdk-content
description: The SetPrompt method sets the text displayed in the dialog box that prompts the user to select a device.
old-location: picacq\iphotoacquiredeviceselectiondialog_setprompt.htm
old-project: acquisition
ms.assetid: 4685c4b8-8c56-4be1-a73f-6d984449d227
ms.author: windowssdkdev
ms.date: 05/25/2018
ms.keywords: IPhotoAcquireDeviceSelectionDialog interface [Picture Acquisition],SetSubmitButtonText method, IPhotoAcquireDeviceSelectionDialog.SetSubmitButtonText, IPhotoAcquireDeviceSelectionDialog::SetSubmitButtonText, IPhotoAcquireDeviceSelectionDialogSetPrompt, SetSubmitButtonText, SetSubmitButtonText method [Picture Acquisition], SetSubmitButtonText method [Picture Acquisition],IPhotoAcquireDeviceSelectionDialog interface, photoacquire/IPhotoAcquireDeviceSelectionDialog::SetSubmitButtonText, picacq.iphotoacquiredeviceselectiondialog_setprompt
ms.prod: windows
ms.technology: windows-sdk
ms.topic: method
req.header: photoacquire.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
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
req.typenames: USER_INPUT_STRING_TYPE
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	PhotoAcquireUID.lib
-	PhotoAcquireUID.dll
api_name:
-	IPhotoAcquireDeviceSelectionDialog.SetSubmitButtonText
product: Windows
targetos: Windows
req.lib: PhotoAcquireUID.lib
req.dll: 
req.irql: 
req.product: Rights Management Services client 1.0 or later
---

# IPhotoAcquireDeviceSelectionDialog::SetSubmitButtonText


## -description



The <code>SetPrompt</code> method sets the text displayed in the dialog box that prompts the user to select a device.




## -parameters




### -param pszSubmitButtonText






#### - pszPrompt [in]

Pointer to a null-terminated string containing the prompt.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://msdn.microsoft.com/7ec649d2-9fd7-4c07-ad64-f3bc4acfc40d">IPhotoAcquireDeviceSelectionDialog Interface</a>
 

 
