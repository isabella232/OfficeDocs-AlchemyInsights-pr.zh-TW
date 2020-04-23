---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720759"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="44493-102">如何停用外部群組</span><span class="sxs-lookup"><span data-stu-id="44493-102">How to disable External Groups</span></span>

<span data-ttu-id="44493-103">Yammer 外部郵件會套用 Exchange 傳輸規則（ETRs），這是一組主動控制措施，可防止公司資訊共用。</span><span class="sxs-lookup"><span data-stu-id="44493-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="44493-104">為了限制使用者建立外部群組，您必須設定 Exchange 傳輸規則（ETR），然後設定 Yammer 使用 Exchange 傳輸規則來封鎖外部郵件。</span><span class="sxs-lookup"><span data-stu-id="44493-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="44493-105">在 Exchange Online 系統管理中心中建立規則之後，請遵循下列步驟，在 Yammer 中設定要套用的 ETR：</span><span class="sxs-lookup"><span data-stu-id="44493-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="44493-106">以已驗證的系統管理員身分登入 Yammer，然後在**yammer 系統管理中心**中，移至 C**內容\>及安全性安全性設定。**</span><span class="sxs-lookup"><span data-stu-id="44493-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="44493-107">在 [**外部郵件**] 底下，選取 [**在 Yammer 中強制執行您的 Exchange Online exchange Transport Rules （ETRs）]。**</span><span class="sxs-lookup"><span data-stu-id="44493-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="44493-108">選擇 [儲存]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="44493-108">Choose **Save**.</span></span>

<span data-ttu-id="44493-109">如需詳細資訊，請參閱[停用 Yammer 網路中的外部郵件](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)。</span><span class="sxs-lookup"><span data-stu-id="44493-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  