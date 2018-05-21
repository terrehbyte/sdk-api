---
UID: NF:shobjidl_core.IOperationsProgressDialog.StartProgressDialog
title: IOperationsProgressDialog::StartProgressDialog
author: windows-driver-content
description: Starts the specified progress dialog.
old-location: shell\IOperationsProgressDialog_StartProgressDialog.htm
old-project: shell
ms.assetid: 5d6f44e0-259f-42d3-9912-877d90f0e7fc
ms.author: windowsdriverdev
ms.date: 5/16/2018
ms.keywords: IOperationsProgressDialog interface [Windows Shell],StartProgressDialog method, IOperationsProgressDialog.StartProgressDialog, IOperationsProgressDialog::StartProgressDialog, OPPROGDLG_ALLOWUNDO, OPPROGDLG_DEFAULT, OPPROGDLG_DONTDISPLAYDESTPATH, OPPROGDLG_DONTDISPLAYLOCATIONS, OPPROGDLG_DONTDISPLAYSOURCEPATH, OPPROGDLG_ENABLEPAUSE, OPPROGDLG_NOMULTIDAYESTIMATES, PROGDLG_AUTOTIME, PROGDLG_MARQUEEPROGRESS, PROGDLG_MODAL, PROGDLG_NOCANCEL, PROGDLG_NOMINIMIZE, PROGDLG_NOPROGRESSBAR, PROGDLG_NORMAL, PROGDLG_NOTIME, StartProgressDialog, StartProgressDialog method [Windows Shell], StartProgressDialog method [Windows Shell],IOperationsProgressDialog interface, _shell_IOperationsProgressDialog_StartProgressDialog, shell.IOperationsProgressDialog_StartProgressDialog, shobjidl_core/IOperationsProgressDialog::StartProgressDialog
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
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
-	COM
api_location:
-	shobjidl_core.h
api_name:
-	IOperationsProgressDialog.StartProgressDialog
product: Windows
targetos: Windows
req.lib: 
req.dll: 
req.irql: 
req.product: Outlook Express 6.0
---

# IOperationsProgressDialog::StartProgressDialog


## -description


Starts the specified progress dialog.


## -parameters




### -param hwndOwner [in]

Type: <b>HWND</b>

A handle to the parent window.


### -param flags






#### - dwFlags [in]

Type: <b>DWORD</b>

Flags that customize the operation. Note that these flags are declared in Shlobj.h. A combination of the following values:



#### PROGDLG_NORMAL (0x00000000)

Default, normal progress dialog behavior.



#### PROGDLG_MODAL (0x00000001)

The dialog is modal to its <i>hwndOwner</i>. The default setting is modeless.



#### PROGDLG_AUTOTIME (0x00000002)

Update "Line3" text with the time remaining. This flag does not need to be implicitly set because progress dialogs started by <b>IOperationsProgressDialog::StartProgressDialog</b> automatically display the time remaining.



#### PROGDLG_NOTIME (0x00000004)

Do not show the time remaining. We do not recommend setting this flag through <a href="https://msdn.microsoft.com/0d95f407-0e09-441d-b9e2-665995ea1362">IOperationsProgressDialog</a> because it goes against the purpose of the dialog.



#### PROGDLG_NOMINIMIZE (0x00000008)

Do not display the minimize button.



#### PROGDLG_NOPROGRESSBAR (0x00000010)

Do not display the progress bar.



#### PROGDLG_MARQUEEPROGRESS (0x00000020)

This flag is invalid in this method. To set the progress bar to marquee mode, use the flags in <a href="https://msdn.microsoft.com/ec731281-c0af-4cf6-aa63-d80a80a18c15">IOperationsProgressDialog::SetMode</a>.



#### PROGDLG_NOCANCEL (0x00000040)

Do not display a cancel button because the operation cannot be canceled. Use this value only when absolutely necessary.



#### OPPROGDLG_DEFAULT (0x00000000)

<b>Windows 7 and later</b>. Indicates default, normal operation progress dialog behavior.



#### OPPROGDLG_ENABLEPAUSE (0x00000080)

Display a pause button. Use this only in situations where the operation can be paused.



#### OPPROGDLG_ALLOWUNDO (0x00000100)

The operation can be undone through the dialog. The <b>Stop</b> button becomes <b>Undo</b>. If pressed, the <b>Undo</b> button then reverts to <b>Stop</b>.



#### OPPROGDLG_DONTDISPLAYSOURCEPATH (0x00000200)

Do not display the path of source file in the progress dialog.



#### OPPROGDLG_DONTDISPLAYDESTPATH (0x00000400)

Do not display the path of the destination file in the progress dialog.



#### OPPROGDLG_NOMULTIDAYESTIMATES (0x00000800)

<b>Windows 7 and later</b>. If the estimated time to completion is greater than one day, do not display the time.



#### OPPROGDLG_DONTDISPLAYLOCATIONS (0x00001000)

<b>Windows 7 and later</b>. Do not display the location line in the progress dialog.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The progress dialog should be created on a separate thread than the file operation on which the dialog is reporting. If the dialog is running in the same thread as the file operation, progress messages are, at best, only sent as resources allow. Progress messages on the same thread as the file operation might not be sent at all.

Once <b>IOperationsProgressDialog::StartProgressDialog</b> is called, that instance of the <b>CLSID_ProgressDialog</b> object cannot be accessed by <a href="https://msdn.microsoft.com/ba0fb1f9-f67f-4cc7-96d8-4c4ccdd213eb">IProgressDialog</a>, <a href="https://msdn.microsoft.com/f3c0e4ae-f93f-4ee2-873a-d9370044e922">IActionProgressDialog</a>, or <a href="https://msdn.microsoft.com/e742e381-0fd2-482a-81a0-7b43d11b073b">IActionProgress</a>. Although <a href="https://msdn.microsoft.com/54d5ff80-18db-43f2-b636-f93ac053146d">QueryInterface</a> can be used to access these interfaces, most of their methods cannot be invoked. <a href="https://msdn.microsoft.com/0d95f407-0e09-441d-b9e2-665995ea1362">IOperationsProgressDialog</a> is the interface used to display the new progress dialog for the Windows Vista and later operations engine.


