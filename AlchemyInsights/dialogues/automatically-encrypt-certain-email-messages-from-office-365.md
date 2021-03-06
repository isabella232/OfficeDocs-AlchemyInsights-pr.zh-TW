---
title: 自動加密 office 365 的特定電子郵件
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509917"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="0a467-102">自動加密 office 365 的特定電子郵件</span><span class="sxs-lookup"><span data-stu-id="0a467-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="0a467-103">從 [Exchange 系統管理中心](https://outlook.office365.com/ecp/)，選擇 [ **郵件流程] > 規則**。</span><span class="sxs-lookup"><span data-stu-id="0a467-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="0a467-104">按一下 [ **新 (+)** ] 圖示，然後按一下 [套用 **Office 365 郵件加密和許可權保護至郵件**]。</span><span class="sxs-lookup"><span data-stu-id="0a467-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="0a467-105">在 [ **名稱**] 中，輸入規則的名稱，例如 [ *加密所有郵件*]。</span><span class="sxs-lookup"><span data-stu-id="0a467-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="0a467-106">在 [套用 **此規則**] 中，選擇 **[套用至所有郵件]**。</span><span class="sxs-lookup"><span data-stu-id="0a467-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="0a467-107">在 [ **執行下列** 欄位] 旁，按一下 [ **選取一個**]。</span><span class="sxs-lookup"><span data-stu-id="0a467-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="0a467-108">在 [ **RMS 範本** ] 下拉式功能表中，選取 [ **加密**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="0a467-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="0a467-109"> (如果您沒有看到此選項，則表示您的計畫不包含自動加密。</span><span class="sxs-lookup"><span data-stu-id="0a467-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="0a467-110">不過，您可以新增！ ) </span><span class="sxs-lookup"><span data-stu-id="0a467-110">But you can add it!)</span></span>
7. <span data-ttu-id="0a467-111">選取 [ **以嚴重性層級審核此規則** ] 核取方塊，然後選取所需的層級。</span><span class="sxs-lookup"><span data-stu-id="0a467-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="0a467-112">如果貴公司有合約，將所有電子郵件都傳送給所有電子郵件，建議將層級設為 **高**。</span><span class="sxs-lookup"><span data-stu-id="0a467-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="0a467-113">在 **[選擇此規則的模型**] 底下，按一下 [ **強制**]。</span><span class="sxs-lookup"><span data-stu-id="0a467-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="0a467-114">從您可以在此位置進行的選用選項清單中選擇任何選擇性選擇 (，許多可以保留預設設定為簡潔性) 。</span><span class="sxs-lookup"><span data-stu-id="0a467-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="0a467-115">按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="0a467-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0a467-116">您隨時可以傳回和編輯此規則。</span><span class="sxs-lookup"><span data-stu-id="0a467-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="0a467-117">如需建立加密規則的相關資訊，請參閱 [定義郵件流程規則以在 Office 365 中加密電子郵件訊息](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="0a467-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

