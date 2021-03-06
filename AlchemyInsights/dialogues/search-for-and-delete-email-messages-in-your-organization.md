---
title: 搜尋並刪除組織中的電子郵件
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500782"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="58990-102">搜尋並刪除組織中的電子郵件</span><span class="sxs-lookup"><span data-stu-id="58990-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="58990-103">請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="58990-103">Follow these steps:</span></span>

1. <span data-ttu-id="58990-104">若您不是全域系統管理員，若要搜尋郵件，您的帳戶必須新增至 **EDiscovery 管理員角色群組** 或 **符合性搜尋管理角色**。</span><span class="sxs-lookup"><span data-stu-id="58990-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="58990-105">若要刪除郵件，您需要加入「 **組織管理」角色群組** 或「 **搜尋並清除」管理角色**。</span><span class="sxs-lookup"><span data-stu-id="58990-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="58990-106">在[安全性 & 規範中心](https://protection.office.com)指派這些角色的許可權。</span><span class="sxs-lookup"><span data-stu-id="58990-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="58990-107">[建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search) ，以尋找要刪除的郵件。</span><span class="sxs-lookup"><span data-stu-id="58990-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="58990-108">[連線到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="58990-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="58990-109">如果您使用的是 MFA，請參閱下列指示： [使用多重要素驗證連線至安全性 & 規範中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="58990-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="58990-110">刪除郵件：執行 `New-ComplianceSearchAction` Cmdlet 以刪除郵件。</span><span class="sxs-lookup"><span data-stu-id="58990-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="58990-111">已刪除的郵件會移至使用者的 [可復原的項目] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="58990-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="58990-112">如需範例命令，請參閱 [Step 3： Delete the message。](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="58990-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
