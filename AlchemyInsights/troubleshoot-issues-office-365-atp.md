---
title: 'Microsoft Defender for Office 365 的問題疑難排解 (ATP) '
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801398"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c95d7-102">疑難排解 Office 365 ATP 的問題</span><span class="sxs-lookup"><span data-stu-id="c95d7-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c95d7-103">**請注意電子郵件傳遞是否延遲** ？</span><span class="sxs-lookup"><span data-stu-id="c95d7-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="c95d7-104">嘗試針對您的 ATP 安全附件原則使用動態傳遞選項。</span><span class="sxs-lookup"><span data-stu-id="c95d7-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c95d7-105">這樣可避免電子郵件傳遞延遲，同時也會防止收件者受到惡意檔案的傳遞。</span><span class="sxs-lookup"><span data-stu-id="c95d7-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c95d7-106">**您是否想要報告誤報或漏報** ？</span><span class="sxs-lookup"><span data-stu-id="c95d7-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="c95d7-107">使用此連結提交您的檔案進行分析： [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c95d7-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c95d7-108">**您是否知道您可以為組織中的人員所傳送的電子郵件啟用 ATP 安全連結保護** ？</span><span class="sxs-lookup"><span data-stu-id="c95d7-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="c95d7-109">請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c95d7-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c95d7-110">移至 https://protection.office.com 並登入。</span><span class="sxs-lookup"><span data-stu-id="c95d7-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c95d7-111">移至 **威脅管理**  >  **原則**  >  **安全連結** 。</span><span class="sxs-lookup"><span data-stu-id="c95d7-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="c95d7-112">在 [套用至特定收件者 **的原則** ] 底下，編輯 (或新增) 原則。</span><span class="sxs-lookup"><span data-stu-id="c95d7-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c95d7-113">選取 **[套用安全連結] 至組織內所傳送的郵件** 。</span><span class="sxs-lookup"><span data-stu-id="c95d7-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="c95d7-114">儲存原則，並允許大約30分鐘的變更，以透過您的資料中心來運作。</span><span class="sxs-lookup"><span data-stu-id="c95d7-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c95d7-115">若要取得其他有關 ATP 的說明，請參閱 [Microsoft Defender For Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)。</span><span class="sxs-lookup"><span data-stu-id="c95d7-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>