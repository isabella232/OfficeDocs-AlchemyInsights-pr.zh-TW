---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704119"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6e58d-102">如何停用外部群組</span><span class="sxs-lookup"><span data-stu-id="6e58d-102">How to disable External Groups</span></span>

<span data-ttu-id="6e58d-103">Yammer 外部郵件會套用 Exchange Transport Rules (ETRs) ，這是一組主動控制措施，可防止公司資訊共用。</span><span class="sxs-lookup"><span data-stu-id="6e58d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="6e58d-104">為了限制使用者建立外部群組，您必須設定 Exchange transport rule (ETR) ，然後設定 Yammer 使用 Exchange 傳輸規則來封鎖外部郵件。</span><span class="sxs-lookup"><span data-stu-id="6e58d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="6e58d-105">在 Exchange Online 系統管理中心中建立規則之後，請遵循下列步驟，在 Yammer 中設定要套用的 ETR：</span><span class="sxs-lookup"><span data-stu-id="6e58d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6e58d-106">以已驗證的系統管理員身分登入 Yammer，然後在 **yammer 系統管理中心**中，移至 C **內容及安全性 \> 安全性設定。**</span><span class="sxs-lookup"><span data-stu-id="6e58d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="6e58d-107">在 [ **外部郵件**] 底下，選取 [在 **Yammer 中執行您的 Exchange Online exchange Transport Rules (ETRs) ]。**</span><span class="sxs-lookup"><span data-stu-id="6e58d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="6e58d-108">選擇 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="6e58d-108">Choose **Save**.</span></span>

<span data-ttu-id="6e58d-109">如需詳細資訊，請參閱 [停用 Yammer 網路中的外部郵件](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)。</span><span class="sxs-lookup"><span data-stu-id="6e58d-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  