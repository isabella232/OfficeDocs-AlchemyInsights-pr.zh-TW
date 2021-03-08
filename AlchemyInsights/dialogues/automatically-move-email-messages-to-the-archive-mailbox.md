---
title: 自動將電子郵件移至封存信箱
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522364"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="90572-102">自動將電子郵件移至封存信箱</span><span class="sxs-lookup"><span data-stu-id="90572-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="90572-103">以下說明如何設定原則，以自動將使用者的舊電子郵件移至封存信箱：</span><span class="sxs-lookup"><span data-stu-id="90572-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="90572-104">移至 [**安全性 & 合規性**](https://go.microsoft.com/fwlink/p/?linkid=2077143)資料控管封存  >    >   ，以確認使用者已啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="90572-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="90572-105">若尚未使用，按一下 [警告] 方塊中的 [ **啟用** ]，然後按一下 [ **是]** 。</span><span class="sxs-lookup"><span data-stu-id="90572-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="90572-106">移至 [**Exchange 系統管理中心 > 合規性管理 > 保留標記**](https://go.microsoft.com/fwlink/?linkid=2059104)。</span><span class="sxs-lookup"><span data-stu-id="90572-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="90572-107">選擇 [+] 圖示，然後選擇 [ **自動套用至整個信箱**]。</span><span class="sxs-lookup"><span data-stu-id="90572-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="90572-108">將名稱指派給保留標記，然後選擇 [ **移至** 封存]。</span><span class="sxs-lookup"><span data-stu-id="90572-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="90572-109">在保留期間內，輸入您想要的時間，例如90天。</span><span class="sxs-lookup"><span data-stu-id="90572-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="90572-110">按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="90572-110">Click **Save**.</span></span>
5. <span data-ttu-id="90572-111">現在建立保留原則：選擇 [ **保留** 原則]，然後選擇圖示以新增原則。</span><span class="sxs-lookup"><span data-stu-id="90572-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="90572-112">將名稱指派給保留原則，然後按一下和滾動以尋找並新增您剛才建立的保留標記。</span><span class="sxs-lookup"><span data-stu-id="90572-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="90572-113">按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="90572-113">Click **Save**.</span></span>
7. <span data-ttu-id="90572-114">最後，將保留原則套用至使用者的信箱：仍然在 Exchange 系統管理中心中，移至 [收件者] **[信箱]**  >  \*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="90572-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="90572-115">選擇您要套用原則的所有使用者，然後選擇 [ **編輯** (鉛筆圖示) 。</span><span class="sxs-lookup"><span data-stu-id="90572-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="90572-116">在對話方塊中，按一下 [ **信箱功能**]。</span><span class="sxs-lookup"><span data-stu-id="90572-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="90572-117">在 [ **保留原則**] 下，套用您剛才建立的原則 > **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="90572-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="90572-118">如需將原則套用至所有使用者的指示，請參閱 [將保留原則套用至信箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。</span><span class="sxs-lookup"><span data-stu-id="90572-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
