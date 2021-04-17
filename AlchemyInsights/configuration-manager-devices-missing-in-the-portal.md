---
title: 入口網站中的 Configuration Manager 裝置遺失
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817235"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="d2efc-102">入口網站中的 Configuration Manager 裝置遺失</span><span class="sxs-lookup"><span data-stu-id="d2efc-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="d2efc-103">若要讓裝置同步處理能夠正常運作，必須從主控服務連線點角色的內部部署伺服器中取得[必要的網際網路端點](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="d2efc-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="d2efc-104">若要疑難排解裝置同步處理，請參閱位於服務連線點上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="d2efc-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="d2efc-105">深入了解 [Microsoft 端點管理員中的租用戶附加](https://docs.microsoft.com/configmgr/tenant-attach/)。</span><span class="sxs-lookup"><span data-stu-id="d2efc-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
