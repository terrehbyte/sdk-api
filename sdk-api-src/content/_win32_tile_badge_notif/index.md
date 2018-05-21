---
UID: TP:win32_tile_badge_notif
ms.assetid: bf033213-8224-36c1-8e23-ab8119b3f34e
ms.author: windowsdriverdev
ms.date: 05/21/18
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: portal
archived: true
---

# Tiles, badges, and notifications for Classic desktop applications



Overview of the Tiles, badges, and notifications for Classic desktop applications technology.

To develop Tiles, badges, and notifications for Classic desktop applications, you need these headers:

 * [notificationactivationcallback.h](..\notificationactivationcallback\index.md)

For the programming guide, see [Tiles, badges, and notifications for Classic desktop applications](https://review.docs.microsoft.com/en-us/win32-test/win32_tile_badge_notif).

## Structures

| Title   | Description   |
| ---- |:---- |
| [NOTIFICATION_USER_INPUT_DATA structure](..\notificationactivationcallback\ns-notificationactivationcallback-notification_user_input_data.md) | Contains information about how a user interacted with a notification toast in the action center. This structure is used by Activate. |

## Interfaces

| Title   | Description   |
| ---- |:---- |
| [INotificationActivationCallback interface](..\notificationactivationcallback\nn-notificationactivationcallback-inotificationactivationcallback.md) | Receives notification messages when an app is triggered through a toast from the action center. |

## Methods

| Title   | Description   |
| ---- |:---- |
| [INotificationActivationCallback::Activate](..\notificationactivationcallback\nf-notificationactivationcallback-inotificationactivationcallback-activate.md) | Called when a user interacts with a toast in the action center. |