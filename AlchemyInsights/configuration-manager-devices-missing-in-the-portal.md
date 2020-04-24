---
title: 入口網站中的 Configuration Manager 裝置遺失
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789601"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="704e0-102">入口網站中的 Configuration Manager 裝置遺失</span><span class="sxs-lookup"><span data-stu-id="704e0-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="704e0-103">若要讓裝置同步處理能夠正常運作，必須從主控服務連線點角色的內部部署伺服器中取得[必要的網際網路端點](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="704e0-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="704e0-104">若要疑難排解裝置同步處理，請參閱位於服務連線點上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="704e0-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="704e0-105">深入了解 [Microsoft 端點管理員中的租用戶附加](https://docs.microsoft.com/configmgr/tenant-attach/)。</span><span class="sxs-lookup"><span data-stu-id="704e0-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
