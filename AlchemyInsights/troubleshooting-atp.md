---
title: 疑難排解 Office 365 高級威脅防護
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658905"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="62971-102">疑難排解 Office 365 高級威脅防護</span><span class="sxs-lookup"><span data-stu-id="62971-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="62971-103">您注意到郵件傳遞中的延遲嗎？</span><span class="sxs-lookup"><span data-stu-id="62971-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="62971-104">使用 ATP 安全附件原則中的 [動態傳遞](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) 選項。</span><span class="sxs-lookup"><span data-stu-id="62971-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="62971-105">這會協助避免郵件延遲，避免來自惡意檔的收件者。</span><span class="sxs-lookup"><span data-stu-id="62971-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="62971-106">您是否要向 Microsoft 報告誤報或漏報？</span><span class="sxs-lookup"><span data-stu-id="62971-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="62971-107">使用此 [連結](https://www.microsoft.com/wdsi/filesubmission/) 提交檔案以進行分析。</span><span class="sxs-lookup"><span data-stu-id="62971-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="62971-108">您是否知道您可以為組織內收件者之間傳送的內部電子郵件啟用安全連結保護？</span><span class="sxs-lookup"><span data-stu-id="62971-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="62971-109">依照下列步驟執行：</span><span class="sxs-lookup"><span data-stu-id="62971-109">Follow these steps:</span></span>

  1. <span data-ttu-id="62971-110">移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="62971-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="62971-111">在 [ **威脅管理**] 底下的左側流覽窗格中，選擇 [ **原則** \> **安全連結**]。</span><span class="sxs-lookup"><span data-stu-id="62971-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="62971-112">在 [ **適用于整個組織的原則** ] 區段中，選取原則，然後按一下 [ **編輯**]。</span><span class="sxs-lookup"><span data-stu-id="62971-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="62971-113">在 [ **設定**] 底下，啟用 **[對組織內傳送的郵件套用安全連結**]。</span><span class="sxs-lookup"><span data-stu-id="62971-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
