---
title: 行事曆圖示沒有顯示在 Teams 用戶端
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819944"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>行事曆圖示沒有顯示在 Teams 用戶端

Teams 中的 [行事曆] 索引標籤需要透過 Exchange Web 服務存取 Exchange 信箱。 Exchange 信箱可以線上或內部部署。 如果您沒有看到 [行事曆] 索引標籤的線上使用者，請確認他們[已取得 Exchange Online 信箱的授權，且已啟用信箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。

如果使用者在 Exchange Online 中有有效的信箱，但仍無法看到 [行事曆] 索引標籤，可能是因為網路問題。 使用 [Microsoft 遠端連線分析程式](https://testconnectivity.microsoft.com/)，並針對受影響的使用者執行 **Microsoft Exchange Web 服務連線測試**。

最後，請檢查 [Teams App – App 設定原則](https://admin.teams.microsoft.com/policies/app-setup)，以確保尚未從應用至使用者的原則中移除行事曆應用程式 (很可能是 **全域 (全組織預設值)**)。

如果您的使用者是位於內部部署的，您必須確認您的混合式組態狀況良好。 使用[混合組態精靈](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) 進行疑難排解。

請注意，[Teams 需要有 Exchange 2016 CU3 或更新版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。
