---
title: 疑難排解 Office 365 高級威脅防護
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512581"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="60c18-102">疑難排解 Office 365 高級威脅防護</span><span class="sxs-lookup"><span data-stu-id="60c18-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="60c18-103">您注意到郵件傳遞中的延遲嗎？</span><span class="sxs-lookup"><span data-stu-id="60c18-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="60c18-104">使用 ATP 安全附件原則中的[動態傳遞](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing)選項。</span><span class="sxs-lookup"><span data-stu-id="60c18-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="60c18-105">這會協助避免郵件延遲，避免來自惡意檔的收件者。</span><span class="sxs-lookup"><span data-stu-id="60c18-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="60c18-106">您是否要向 Microsoft 報告誤報或漏報？</span><span class="sxs-lookup"><span data-stu-id="60c18-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="60c18-107">使用此[連結](https://www.microsoft.com/wdsi/filesubmission/)提交檔案以進行分析。</span><span class="sxs-lookup"><span data-stu-id="60c18-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="60c18-108">您是否知道您可以為組織內收件者之間傳送的內部電子郵件啟用安全連結保護？</span><span class="sxs-lookup"><span data-stu-id="60c18-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="60c18-109">請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="60c18-109">Follow these steps:</span></span>

  1. <span data-ttu-id="60c18-110">移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="60c18-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="60c18-111">在 [**威脅管理**] 底下的左側流覽窗格中，選擇 [**原則** \> **安全連結**]。</span><span class="sxs-lookup"><span data-stu-id="60c18-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="60c18-112">在 [**適用于整個組織的原則**] 區段中，選取原則，然後按一下 [**編輯**]。</span><span class="sxs-lookup"><span data-stu-id="60c18-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="60c18-113">在 [**設定**] 底下，啟用 **[對組織內傳送的郵件套用安全連結**]。</span><span class="sxs-lookup"><span data-stu-id="60c18-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
