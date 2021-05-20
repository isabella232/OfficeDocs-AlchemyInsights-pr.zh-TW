---
title: Office 365 的 Microsoft Defender 疑難排解
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545259"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="4d8a9-102">Office 365 的 Microsoft Defender 疑難排解</span><span class="sxs-lookup"><span data-stu-id="4d8a9-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="4d8a9-103">**您注意到郵件傳遞中的延遲嗎？**</span><span class="sxs-lookup"><span data-stu-id="4d8a9-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="4d8a9-104">在您的 Microsoft Defender 中使用[動態傳遞](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing)選項，以 Office 365 安全附件原則。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="4d8a9-105">這會協助避免郵件延遲，避免來自惡意檔的收件者。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="4d8a9-106">**您是否要向 Microsoft 報告誤報或漏報？**</span><span class="sxs-lookup"><span data-stu-id="4d8a9-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="4d8a9-107">使用 [提交的 Explorer](https://protection.office.com/reportsubmission)。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="4d8a9-108">-\* \* 您是否知道您可以為組織內收件者之間傳送的內部電子郵件啟用安全連結保護？ \* \* 請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="4d8a9-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="4d8a9-109">移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="4d8a9-110">在 [ **威脅管理**] 底下的左側流覽窗格中，選擇 [ **原則** \> **安全連結**]。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="4d8a9-111">在 [ **適用于整個組織的原則** ] 區段中，選取原則，然後按一下 [ **編輯**]。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="4d8a9-112">在 [**設定**] 底下，啟用 **[套用安全連結至組織內傳送的郵件**]。</span><span class="sxs-lookup"><span data-stu-id="4d8a9-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
