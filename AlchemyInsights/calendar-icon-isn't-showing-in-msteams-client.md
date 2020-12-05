---
title: 在 Microsoft 團隊用戶端中未顯示行事曆圖示
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576428"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="c40e2-102">在 Microsoft 團隊用戶端中未顯示行事曆圖示</span><span class="sxs-lookup"><span data-stu-id="c40e2-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="c40e2-103">小組中的 [行事 **曆** ] 索引標籤需要透過 Exchange Web 服務存取 exchange 信箱。</span><span class="sxs-lookup"><span data-stu-id="c40e2-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="c40e2-104">Exchange 信箱可以是線上或 On-Premises。</span><span class="sxs-lookup"><span data-stu-id="c40e2-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="c40e2-105">對於未看到 [行事 **曆** ] 索引標籤的線上使用者，請確定他們 [已獲得 Exchange Online 信箱的授權，且已啟用信箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="c40e2-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="c40e2-106">如果您的使用者已 On-Premises，您必須確認您的混合式設定狀況良好。</span><span class="sxs-lookup"><span data-stu-id="c40e2-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="c40e2-107">使用[混合組態精靈](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) 進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="c40e2-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="c40e2-108">請注意，[Teams 需要有 Exchange 2016 CU3 或更新版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。</span><span class="sxs-lookup"><span data-stu-id="c40e2-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="c40e2-109">如需詳細資訊及疑難排解步驟，請參閱 [疑難排解 Microsoft 團隊和 Exchange Server 互動問題](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)。</span><span class="sxs-lookup"><span data-stu-id="c40e2-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
