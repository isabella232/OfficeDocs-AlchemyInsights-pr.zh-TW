---
title: 不顯示敏感度標籤
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801175"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="6b072-102">不顯示敏感度標籤</span><span class="sxs-lookup"><span data-stu-id="6b072-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="6b072-103">敏感度標籤可讓您分類並協助保護您的敏感內容。</span><span class="sxs-lookup"><span data-stu-id="6b072-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="6b072-104">您可以在 [分類 > 敏感度標籤] 底下的 [microsoft 365 規範中心]、[Microsoft 365 安全性中心] 或 [Microsoft 365 安全性 & 規範中心] 中建立。</span><span class="sxs-lookup"><span data-stu-id="6b072-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="6b072-105">若要深入瞭解這項功能，請參閱 [敏感度標籤簡介](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)。</span><span class="sxs-lookup"><span data-stu-id="6b072-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="6b072-106">如果您已設定靈敏度標籤，但未出現在 Microsoft 365 應用程式中，請檢查下列各項：</span><span class="sxs-lookup"><span data-stu-id="6b072-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="6b072-107">確認敏感度標籤已 [發佈](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) 至您想要的使用者和群組。</span><span class="sxs-lookup"><span data-stu-id="6b072-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="6b072-108">確認使用者正在使用支援敏感度標籤的應用程式-請參閱 [檔中的靈敏度標籤](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)。</span><span class="sxs-lookup"><span data-stu-id="6b072-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="6b072-109">如果您要 [遷移 Azure 資訊保護標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)，請注意 [這裡](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)所列的考慮。</span><span class="sxs-lookup"><span data-stu-id="6b072-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="6b072-110">資料遺失防護 (DLP) 支援：目前，只有保留標籤可以作為 DLP 原則中的條件使用。</span><span class="sxs-lookup"><span data-stu-id="6b072-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="6b072-111">無法使用 DLP 原則中的靈敏度標籤，但我們正在處理。</span><span class="sxs-lookup"><span data-stu-id="6b072-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="6b072-112">在敏感度標籤上啟用加密時，您可以選擇：</span><span class="sxs-lookup"><span data-stu-id="6b072-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="6b072-113">立即指派權限</span><span class="sxs-lookup"><span data-stu-id="6b072-113">Assign permissions now</span></span>
    - <span data-ttu-id="6b072-114">讓使用者指派權限</span><span class="sxs-lookup"><span data-stu-id="6b072-114">Let users assign permissions</span></span>


<span data-ttu-id="6b072-115">如需可能問題的詳細資訊，請參閱 [敏感性標籤的已知問題](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)。</span><span class="sxs-lookup"><span data-stu-id="6b072-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>