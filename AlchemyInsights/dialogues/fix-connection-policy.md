---
title: 修正連接原則
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568495"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="0692e-102">修正連接原則</span><span class="sxs-lookup"><span data-stu-id="0692e-102">Fix connection policy</span></span>

<span data-ttu-id="0692e-103">電子郵件已標示為安全，並傳遞至使用者的收件匣，因為在連線篩選原則中已標示為安全的傳送 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="0692e-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="0692e-104">若要查看原則，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="0692e-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="0692e-105">移至 [Office 365 Security & 合規性中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)，然後移至 **威脅管理**  >  **原則**  >  [反垃圾郵件](https://go.microsoft.com/fwlink/?linkid=2101518)。</span><span class="sxs-lookup"><span data-stu-id="0692e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="0692e-106">在 [ **自訂** ] 索引標籤上，選取連線 **篩選原則**，然後選取 [ **編輯原則**]。</span><span class="sxs-lookup"><span data-stu-id="0692e-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="0692e-107">複查 [ **IP 允許** ] 清單。</span><span class="sxs-lookup"><span data-stu-id="0692e-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="0692e-108">請參閱是否已啟用 **安全清單** 。</span><span class="sxs-lookup"><span data-stu-id="0692e-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0692e-109">Microsoft 會訂閱協力廠商來源的信任寄件者。</span><span class="sxs-lookup"><span data-stu-id="0692e-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="0692e-110">如果啟用 **安全清單** ，這些受信任的寄件者不會錯誤地標示為垃圾郵件。</span><span class="sxs-lookup"><span data-stu-id="0692e-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="0692e-111">我建議選取此選項，因為它會減少誤報數目 (很棒的郵件會被分類為您收到的垃圾郵件) 。</span><span class="sxs-lookup"><span data-stu-id="0692e-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
