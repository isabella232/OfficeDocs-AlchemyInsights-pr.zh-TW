---
title: Microsoft Defender for Office 365 反網路釣魚原則範例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552326"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="298e4-102">Microsoft Defender for Office 365 反網路釣魚原則範例</span><span class="sxs-lookup"><span data-stu-id="298e4-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="298e4-103">這些設定會啟用名為 *Domain 及 CEO* 的原則。</span><span class="sxs-lookup"><span data-stu-id="298e4-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="298e4-104">這個原則提供使用者和網域保護的模擬，然後將該原則套用至網域中使用者所收到的所有電子郵件。</span><span class="sxs-lookup"><span data-stu-id="298e4-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="298e4-105">首先，新增下列資訊以建立原則：</span><span class="sxs-lookup"><span data-stu-id="298e4-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="298e4-106">**名稱**：網域與 CEO **描述**：確保 CEO 和您的網域未進行類比。</span><span class="sxs-lookup"><span data-stu-id="298e4-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="298e4-107">**適用** 于：選取 **[收件者網域**]。</span><span class="sxs-lookup"><span data-stu-id="298e4-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="298e4-108">在 [ **任何**] 底下，選取 **[選擇**]，然後選取網域。</span><span class="sxs-lookup"><span data-stu-id="298e4-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="298e4-109">選取 **[+ 新增]**。</span><span class="sxs-lookup"><span data-stu-id="298e4-109">Select **+ Add**.</span></span> <span data-ttu-id="298e4-110">選取清單中網功能變數名稱稱旁邊的核取方塊 (例如， *contoso.com*) ]，然後選取 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="298e4-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="298e4-111">選取 **[完成]**。</span><span class="sxs-lookup"><span data-stu-id="298e4-111">Select **Done**.</span></span>
- <span data-ttu-id="298e4-112">建立原則之後，您可以使用下列選項微調原則：</span><span class="sxs-lookup"><span data-stu-id="298e4-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="298e4-113">**新增要保護的使用者：** 在此範例中，至少要新增 CEO 的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="298e4-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="298e4-114">**新增要保護的網域**：新增包含 CEO 的 office 的組織網域。</span><span class="sxs-lookup"><span data-stu-id="298e4-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="298e4-115">**選擇動作**：若要讓模擬的 **使用者傳送電子郵件**，請選取 [ **將郵件重新導向至另一個電子郵件地址**]，然後輸入安全性管理員 (的電子郵件地址，例如， *securityadmin@contoso.com*) 。</span><span class="sxs-lookup"><span data-stu-id="298e4-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="298e4-116">**若為類比網域傳送電子郵件**，請選取 **[隔離郵件**]。</span><span class="sxs-lookup"><span data-stu-id="298e4-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="298e4-117">**信箱智慧**：根據預設，當您建立新的反網路釣魚原則時，會選取此選項。</span><span class="sxs-lookup"><span data-stu-id="298e4-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="298e4-118">請將此設定保留為 **[開啟]**，以獲得最佳結果。</span><span class="sxs-lookup"><span data-stu-id="298e4-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="298e4-119">**新增信任的寄件者和網域：** 在此範例中，請勿定義任何覆寫。</span><span class="sxs-lookup"><span data-stu-id="298e4-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="298e4-120">檢查您的設定之後，請選取 [ **建立這個原則** ] 或 [ **儲存**] （視需要）。</span><span class="sxs-lookup"><span data-stu-id="298e4-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="298e4-121">若要深入瞭解，請參閱 [Microsoft 365 中的反網路釣魚原則](https://go.microsoft.com/fwlink/?linkid=2092235)。</span><span class="sxs-lookup"><span data-stu-id="298e4-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
