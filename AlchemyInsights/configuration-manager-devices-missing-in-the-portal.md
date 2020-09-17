---
title: 入口網站中的 Configuration Manager 裝置遺失
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812142"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="6c4db-102">入口網站中的 Configuration Manager 裝置遺失</span><span class="sxs-lookup"><span data-stu-id="6c4db-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="6c4db-103">若要讓裝置同步處理能夠正常運作，必須從主控服務連線點角色的內部部署伺服器中取得[必要的網際網路端點](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="6c4db-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="6c4db-104">若要疑難排解裝置同步處理，請參閱位於服務連線點上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="6c4db-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="6c4db-105">深入了解 [Microsoft 端點管理員中的租用戶附加](https://docs.microsoft.com/configmgr/tenant-attach/)。</span><span class="sxs-lookup"><span data-stu-id="6c4db-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
