---
title: Outlook 網頁版中的 S/MIME
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752851"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="7e9f7-102">在 Outlook 中的電子郵件加密</span><span class="sxs-lookup"><span data-stu-id="7e9f7-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="7e9f7-103">Office 365 郵件加密是內建於 Microsoft Azure 版權管理 (Azure RMS)，也就是 Azure 資訊保護的一部分。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="7e9f7-104">如果您的訂閱包含 Azure 版權管理 」 或 「 Azure 資訊保護，**您不需要採取任何動作，以手動啟用或啟動**版權管理服務。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="7e9f7-105">根據客戶意見反應，我們將不再讓 Exchange 郵件流程規則來自動加密預設包含特定類型的租用戶中的敏感資訊的外寄電子郵件。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="7e9f7-106">相反地，我們會提供的詳細的指示上如何可以進行自己。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="7e9f7-107">如需如何建立傳輸規則以加密敏感資訊的其他詳細資訊，請參閱[這篇文章](https://aka.ms/OmeEtr)。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="7e9f7-108">如果使用 Outlook 網頁 (先前稱為**OWA**): 當您在撰寫電子郵件，只要按一下 [在 OWA 中的**保護**。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="7e9f7-109">這將會套用 「 不要轉寄 」 權限。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="7e9f7-110">按一下 [**變更權限**，然後選擇 [僅加密訊息**加密**。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="7e9f7-111">如果使用**Outlook 用戶端**： 從來傳送加密的郵件 Outlook 2013 或 2016 或 Outlook 2016 for Mac 中，選取 [**選項** > **權限**，然後選取您需要的保護選項。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="7e9f7-112">若要**自動加密所有電子郵件**傳送給特定收件者或外部夥伴組織，您需要在 Exchange 系統管理中心中建立郵件流程傳輸規則。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="7e9f7-113">[支援本文](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)所提供的詳細的指示。</span><span class="sxs-lookup"><span data-stu-id="7e9f7-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

