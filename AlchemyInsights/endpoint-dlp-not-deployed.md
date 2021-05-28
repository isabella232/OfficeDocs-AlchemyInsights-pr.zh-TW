---
title: 端點 DLP 未部署至使用者的裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694802"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="cf9d4-102">端點 DLP 未部署至使用者的裝置</span><span class="sxs-lookup"><span data-stu-id="cf9d4-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="cf9d4-103">如果端點資料外洩防護 (DLP) 設定尚未套用至使用者的裝置，請確認您符合這些需求：</span><span class="sxs-lookup"><span data-stu-id="cf9d4-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="cf9d4-104">Windows 10 x64 組建 1809 或更新版本已安裝在裝置上。</span><span class="sxs-lookup"><span data-stu-id="cf9d4-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="cf9d4-105">已安裝反惡意程式碼用戶端版本 4.18.2009.7 或更新版本。</span><span class="sxs-lookup"><span data-stu-id="cf9d4-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="cf9d4-106">裝置為以下 **其中一種**：</span><span class="sxs-lookup"><span data-stu-id="cf9d4-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="cf9d4-107">已使用 Azure Active Directory (Azure AD) 而聯結的</span><span class="sxs-lookup"><span data-stu-id="cf9d4-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="cf9d4-108">已使用混合式 Azure AD 而聯結的</span><span class="sxs-lookup"><span data-stu-id="cf9d4-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="cf9d4-109">AAD 已註冊</span><span class="sxs-lookup"><span data-stu-id="cf9d4-109">AAD registered</span></span>

- <span data-ttu-id="cf9d4-110">若要強制執行原則動作，請確定端點裝置上已安裝 Microsoft Chromium Edge 瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="cf9d4-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="cf9d4-111">如需部署端點 DLP 的其他需求，請參閱[開始使用端點資料外洩防護](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="cf9d4-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>