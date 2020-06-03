---
title: Outlook 網頁版中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511499"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="cf913-102">加密 Outlook 中的電子郵件</span><span class="sxs-lookup"><span data-stu-id="cf913-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="cf913-103">Microsoft 365 郵件加密是以 Microsoft Azure Rights Management （Azure RMS）為基礎，這是 Azure 資訊保護的一部分。</span><span class="sxs-lookup"><span data-stu-id="cf913-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="cf913-104">如果您的訂閱包含 Azure 版權管理或 Azure 資訊保護，**您不需要採取任何動作手動啟用或啟用**Rights Management 服務。</span><span class="sxs-lookup"><span data-stu-id="cf913-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="cf913-105">根據客戶的意見反應，我們將不再啟用 Exchange 郵件流程規則，以預設會在您的租使用者中自動加密包含特定類型敏感資訊的輸出電子郵件。</span><span class="sxs-lookup"><span data-stu-id="cf913-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="cf913-106">相反地，我們會提供如何進行此作業的詳細指示。</span><span class="sxs-lookup"><span data-stu-id="cf913-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="cf913-107">如需如何建立傳輸規則以加密機密資訊的其他詳細資料，請參閱[本文](https://aka.ms/OmeEtr)。</span><span class="sxs-lookup"><span data-stu-id="cf913-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="cf913-108">如果使用網頁上的 Outlook （以前稱為**OWA**）：撰寫電子郵件時，只要按一下 OWA 中的 [**保護**] 即可。</span><span class="sxs-lookup"><span data-stu-id="cf913-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="cf913-109">這將會套用「不要轉寄」許可權。</span><span class="sxs-lookup"><span data-stu-id="cf913-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="cf913-110">按一下 [**變更許可權**]，然後選擇 [**加密**] 以只加密郵件。</span><span class="sxs-lookup"><span data-stu-id="cf913-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="cf913-111">若使用**outlook 用戶端**：若要從 outlook 2013 或2016（或 outlook 2016 Mac）傳送加密的郵件，請選取 [**選項**  >  **許可權**]，然後選取所需的保護選項。</span><span class="sxs-lookup"><span data-stu-id="cf913-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="cf913-112">若要**自動加密所有**傳送給特定收件者或外部夥伴組織的電子郵件，您必須在 Exchange 系統管理中心中建立郵件流程傳輸規則。</span><span class="sxs-lookup"><span data-stu-id="cf913-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="cf913-113">[此支援文章](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)中提供詳細指示。</span><span class="sxs-lookup"><span data-stu-id="cf913-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

