---
title: 在 Microsoft Edge 中設定隱私權設定
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403814"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="d669b-102">在 Microsoft Edge 中設定隱私權設定</span><span class="sxs-lookup"><span data-stu-id="d669b-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="d669b-103">根據預設，如果 Microsoft Edge 部署在非 Windows 平臺上，則診斷資料和網站資訊不會傳送給 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="d669b-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="d669b-104">不過，如果 Microsoft Edge 部署在 Windows 10 上，診斷資料和網站資訊會根據使用者的 [Windows 診斷資料設定](https://go.microsoft.com/fwlink/?linkid=2132472)傳送。</span><span class="sxs-lookup"><span data-stu-id="d669b-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="d669b-105">若要設定 Microsoft Edge 如何處理組織的資料收集，請使用下列群組原則：</span><span class="sxs-lookup"><span data-stu-id="d669b-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="d669b-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) 開啟使用狀況和崩潰相關資料的報告。</span><span class="sxs-lookup"><span data-stu-id="d669b-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="d669b-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) 會傳送用來改善 Microsoft 服務的網站資訊。</span><span class="sxs-lookup"><span data-stu-id="d669b-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="d669b-108">若要深入瞭解，請參閱 [設定原則設定](https://go.microsoft.com/fwlink/?linkid=2132577)。</span><span class="sxs-lookup"><span data-stu-id="d669b-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
