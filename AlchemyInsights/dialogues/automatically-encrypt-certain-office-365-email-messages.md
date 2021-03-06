---
title: 自動加密某些 Office 365 電子郵件
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509911"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="c5485-102">自動加密某些 Office 365 電子郵件</span><span class="sxs-lookup"><span data-stu-id="c5485-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="c5485-103">您可以自動加密使用者傳送給特定外部人員或組織的郵件。</span><span class="sxs-lookup"><span data-stu-id="c5485-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="c5485-104">若要執行此動作，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c5485-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="c5485-105">從 [Exchange 系統管理中心](https://outlook.office365.com/ecp/)，選擇 [ **郵件流程] > 規則**。</span><span class="sxs-lookup"><span data-stu-id="c5485-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c5485-106">按一下 [ **新 (+)** ] 圖示，然後按一下 [套用 **Office 365 郵件加密和許可權保護至郵件**]。</span><span class="sxs-lookup"><span data-stu-id="c5485-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c5485-107">在 [ **名稱**] 中，輸入規則的名稱，例如 [ *加密傳送至 DrToniRamos@gmail.com 的郵件*]。</span><span class="sxs-lookup"><span data-stu-id="c5485-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="c5485-108">在 [套用 **此規則**] 中，選擇 **[收件者] > 為此人員**。</span><span class="sxs-lookup"><span data-stu-id="c5485-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="c5485-109">在 [ **選取成員** ] 視窗中，選取您要套用加密規則的人員名稱，然後按一下 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="c5485-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="c5485-110">當您完成新增使用者時，請按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="c5485-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="c5485-111">在 [ **執行下列** 欄位] 旁，按一下 [ **選取一個**]。</span><span class="sxs-lookup"><span data-stu-id="c5485-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="c5485-112">在 [ **RMS 範本** ] 下拉式功能表中，選取 [ **加密**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="c5485-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c5485-113"> (如果您沒有看到此選項，則表示您的計畫不包含自動加密。</span><span class="sxs-lookup"><span data-stu-id="c5485-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c5485-114">不過，您可以新增！ ) </span><span class="sxs-lookup"><span data-stu-id="c5485-114">But you can add it!)</span></span>
9. <span data-ttu-id="c5485-115">從您可以在此位置進行的選用選項清單中選擇任何選擇性選擇 (，許多可以保留預設設定為簡潔性) 。</span><span class="sxs-lookup"><span data-stu-id="c5485-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c5485-116">按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="c5485-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c5485-117">您隨時可以傳回和編輯此規則。</span><span class="sxs-lookup"><span data-stu-id="c5485-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c5485-118">如需建立加密規則的相關資訊，請參閱 [定義郵件流程規則，以加密 Office 365 中的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。</span><span class="sxs-lookup"><span data-stu-id="c5485-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

