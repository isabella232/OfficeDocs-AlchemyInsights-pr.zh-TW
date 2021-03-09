---
title: '修正承租人原則 (動作覆寫) '
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552330"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="0a3d8-102">修正承租人原則 (動作覆寫) </span><span class="sxs-lookup"><span data-stu-id="0a3d8-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="0a3d8-103">您租使用者中的反垃圾郵件原則會影響此郵件。</span><span class="sxs-lookup"><span data-stu-id="0a3d8-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="0a3d8-104">若要查看原則，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="0a3d8-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="0a3d8-105">移至 [Office 365 Security & 合規性中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)，然後移至 **威脅管理**  >  **原則**  >  [反垃圾郵件](https://go.microsoft.com/fwlink/?linkid=2101518)。</span><span class="sxs-lookup"><span data-stu-id="0a3d8-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="0a3d8-106">查看 [ **原則來源** ] 是否指出下列專案：  **載入 Xheader/ModifySubject/重新導向/刪除/否動作/BCC 郵件**</span><span class="sxs-lookup"><span data-stu-id="0a3d8-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="0a3d8-107">如果是的話，在 [ **自訂** ] 索引標籤上，檢查會影響郵件之原則的設定。</span><span class="sxs-lookup"><span data-stu-id="0a3d8-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="0a3d8-108">適用于所有 Exchange Online Protection 客戶的 **標準設定** 可能會影響郵件。</span><span class="sxs-lookup"><span data-stu-id="0a3d8-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="0a3d8-109">如需設定垃圾郵件篩選原則的詳細資訊，請參閱 [設定垃圾郵件篩選原則](https://go.microsoft.com/fwlink/?linkid=2101431)。</span><span class="sxs-lookup"><span data-stu-id="0a3d8-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
