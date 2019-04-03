---
title: 疑難排解問題與 Office 365 進階威脅防護 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030904"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="0f55d-102">疑難排解 Office 365 ATP 的問題</span><span class="sxs-lookup"><span data-stu-id="0f55d-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="0f55d-103">**電子郵件訊息傳遞的通知延遲**？</span><span class="sxs-lookup"><span data-stu-id="0f55d-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="0f55d-104">請嘗試使用 ATP 安全附件原則的 [動態傳遞] 選項。</span><span class="sxs-lookup"><span data-stu-id="0f55d-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="0f55d-105">這樣可避免電子郵件訊息傳遞延遲同時防止惡意檔案中的收件者。</span><span class="sxs-lookup"><span data-stu-id="0f55d-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="0f55d-106">**您要報告誤判或漏報**嗎？</span><span class="sxs-lookup"><span data-stu-id="0f55d-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="0f55d-107">使用此連結來提交您進行分析的檔案：[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="0f55d-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="0f55d-108">**您知道您可以啟用 ATP 安全連結保護您組織中的人員之間傳送的電子郵件嗎**？</span><span class="sxs-lookup"><span data-stu-id="0f55d-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="0f55d-109">請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="0f55d-109">Follow these steps:</span></span>
    1. <span data-ttu-id="0f55d-110">移至 [ https://protection.office.com，並登入。</span><span class="sxs-lookup"><span data-stu-id="0f55d-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="0f55d-111">移至**威脅管理，** > **原則** > **安全連結**。</span><span class="sxs-lookup"><span data-stu-id="0f55d-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="0f55d-112">[**套用至特定收件者原則**] 下編輯 （或新增） 原則。</span><span class="sxs-lookup"><span data-stu-id="0f55d-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="0f55d-113">選取 [**套用安全連結到組織內傳送的郵件**。</span><span class="sxs-lookup"><span data-stu-id="0f55d-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="0f55d-114">儲存您的原則，並允許大約 30 分鐘，對其透過您的資料中心的方式運作。</span><span class="sxs-lookup"><span data-stu-id="0f55d-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="0f55d-115">若要取得的 ATP 的詳細說明，請參閱[Office 365 進階威脅防護](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)。</span><span class="sxs-lookup"><span data-stu-id="0f55d-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>