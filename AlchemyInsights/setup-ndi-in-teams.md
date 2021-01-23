---
title: 開啟 NDI 技術
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917309"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="4f425-102">開啟 NDI 技術</span><span class="sxs-lookup"><span data-stu-id="4f425-102">Turn on NDI technology</span></span>

<span data-ttu-id="4f425-103">NDI 技術需要為使用者開啟兩個步驟：</span><span class="sxs-lookup"><span data-stu-id="4f425-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="4f425-104">租使用者管理員必須啟用 CsTeamsMeetingPolicy 中的 ' AllowNDIStreaming ' 屬性。</span><span class="sxs-lookup"><span data-stu-id="4f425-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="4f425-105">在此變更填滿後，使用者必須從 [ **設定 > 許可權**] 的特定用戶端開啟 NDI®技術。</span><span class="sxs-lookup"><span data-stu-id="4f425-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="4f425-106">如需詳細資訊，請參閱 [USE NDI 技術協會 In Microsoft 球隊](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)。</span><span class="sxs-lookup"><span data-stu-id="4f425-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
