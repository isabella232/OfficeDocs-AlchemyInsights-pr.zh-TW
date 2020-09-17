---
title: 在傳輸規則中使用 DLP
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
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773154"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="7851f-102">在傳輸規則中使用 DLP</span><span class="sxs-lookup"><span data-stu-id="7851f-102">Using DLP in transport rules</span></span>

<span data-ttu-id="7851f-103">若要將資料遺失防護 (DLP) 整合至現有傳輸，請使用 [傳輸規則] 設定中的**如果郵件包含...機密資訊**條件。</span><span class="sxs-lookup"><span data-stu-id="7851f-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="7851f-104">**如需詳細資訊，請參閱：**</span><span class="sxs-lookup"><span data-stu-id="7851f-104">**For more details, see:**</span></span>

- <span data-ttu-id="7851f-105">傳輸規則中整合的 DLP 機密資訊類型：[整合機密資訊規則](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。</span><span class="sxs-lookup"><span data-stu-id="7851f-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="7851f-106">您也可以使用規則上的測試模式，利用原則測試或不利用原則測試來測試規則。</span><span class="sxs-lookup"><span data-stu-id="7851f-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="7851f-107">建立規則後、測試之前，請先等候 30 分鐘。</span><span class="sxs-lookup"><span data-stu-id="7851f-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="7851f-108">請參閱[測試郵件流程/傳輸規則](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="7851f-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="7851f-109">**注意**：如果您嘗試使用 EAC 中的傳輸規則來實作新的 DLP 原則，請改用[安全性與合規性中心中的 DLP 原則](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="7851f-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
