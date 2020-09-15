---
title: 行事曆圖示沒有顯示在 Teams 用戶端
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
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684689"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="8f9bb-102">行事曆圖示沒有顯示在 Teams 用戶端</span><span class="sxs-lookup"><span data-stu-id="8f9bb-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="8f9bb-103">Teams 中的 [行事曆] 索引標籤需要透過 Exchange Web 服務存取 Exchange 信箱。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="8f9bb-104">Exchange 信箱可以線上或內部部署。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="8f9bb-105">如果您沒有看到 [行事曆] 索引標籤的線上使用者，請確認他們[已取得 Exchange Online 信箱的授權，且已啟用信箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="8f9bb-106">如果使用者在 Exchange Online 中有有效的信箱，但仍無法看到 [行事曆] 索引標籤，可能是因為網路問題。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="8f9bb-107">使用 [Microsoft 遠端連線分析程式](https://testconnectivity.microsoft.com/)，並針對受影響的使用者執行 **Microsoft Exchange Web 服務連線測試**。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="8f9bb-108">最後，請檢查 [Teams App – App 設定原則](https://admin.teams.microsoft.com/policies/app-setup)，以確保尚未從應用至使用者的原則中移除行事曆應用程式 (很可能是**全域 (全組織預設值)**)。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="8f9bb-109">如果您的使用者是位於內部部署的，您必須確認您的混合式組態狀況良好。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="8f9bb-110">使用[混合組態精靈](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) 進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="8f9bb-111">請注意，[Teams 需要有 Exchange 2016 CU3 或更新版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。</span><span class="sxs-lookup"><span data-stu-id="8f9bb-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
