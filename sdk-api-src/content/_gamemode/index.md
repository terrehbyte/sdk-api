---
UID: TP:gamemode
ms.assetid: 7e85c2c5-8d7f-3617-a348-14e79b75cc10
ms.author: windowsdriverdev
ms.date: 05/21/18
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: portal
archived: true
---

# Game Mode



Overview of the Game Mode technology.

To develop Game Mode, you need these headers:

 * [expandedresources.h](..\expandedresources\index.md)

For the programming guide, see [Game Mode](https://review.docs.microsoft.com/en-us/win32-test/gamemode).

## Functions

| Title   | Description   |
| ---- |:---- |
| [GetExpandedResourceExclusiveCpuCount function](..\expandedresources\nf-expandedresources-getexpandedresourceexclusivecpucount.md) | Gets the expected number of exclusive CPU sets that are available to the app when in Game Mode. |
| [HasExpandedResources function](..\expandedresources\nf-expandedresources-hasexpandedresources.md) | Gets the current resource state (that is, whether the app is running in Game Mode or shared mode). |
| [ReleaseExclusiveCpuSets function](..\expandedresources\nf-expandedresources-releaseexclusivecpusets.md) | Opts out of CPU exclusivity, giving the app access to all cores, but at the cost of having to share them with other processes. |