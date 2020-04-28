---
title: 在傳輸規則中使用 DLP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915047"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="b3f24-102">在傳輸規則中使用 DLP</span><span class="sxs-lookup"><span data-stu-id="b3f24-102">Using DLP in transport rules</span></span>

<span data-ttu-id="b3f24-103">若要將資料遺失防護 (DLP) 整合至現有傳輸，請使用 [傳輸規則] 設定中的**如果郵件包含...機密資訊**條件。</span><span class="sxs-lookup"><span data-stu-id="b3f24-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="b3f24-104">**如需詳細資訊，請參閱：**</span><span class="sxs-lookup"><span data-stu-id="b3f24-104">**For more details, see:**</span></span>

- <span data-ttu-id="b3f24-105">傳輸規則中整合的 DLP 機密資訊類型：[整合機密資訊規則](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。</span><span class="sxs-lookup"><span data-stu-id="b3f24-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="b3f24-106">您也可以使用規則上的測試模式，利用原則測試或不利用原則測試來測試規則。</span><span class="sxs-lookup"><span data-stu-id="b3f24-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="b3f24-107">建立規則後、測試之前，請先等候 30 分鐘。</span><span class="sxs-lookup"><span data-stu-id="b3f24-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="b3f24-108">請參閱[測試郵件流程/傳輸規則](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="b3f24-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="b3f24-109">**注意**：如果您嘗試使用 EAC 中的傳輸規則來實作新的 DLP 原則，請改用[安全性與合規性中心中的 DLP 原則](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="b3f24-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
