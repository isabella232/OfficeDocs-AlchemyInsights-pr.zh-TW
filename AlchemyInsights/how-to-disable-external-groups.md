---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399582"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="c897c-102">如何停用外部群組</span><span class="sxs-lookup"><span data-stu-id="c897c-102">How to disable External Groups</span></span>

<span data-ttu-id="c897c-103">Yammer 外部通訊適用於 Exchange 傳輸規則 (Etr)，一組的積極的控制項，以防止使用者從共用的公司資訊。</span><span class="sxs-lookup"><span data-stu-id="c897c-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="c897c-104">若要限制使用者只能建立外部群組，您需要設定 Exchange 傳輸規則 (ETR)，然後再設定 Yammer 可使用 Exchange 傳輸規則，以封鎖外部訊息。</span><span class="sxs-lookup"><span data-stu-id="c897c-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="c897c-105">一旦您在 Exchange Online 系統管理中心建立規則，請遵循下列步驟來設定 ETR 套用在 Yammer 中：</span><span class="sxs-lookup"><span data-stu-id="c897c-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="c897c-106">登入 Yammer 已驗證的系統管理員，並在**Yammer 系統管理中心**，移至 C **ontent 和安全性\>安全性設定。**</span><span class="sxs-lookup"><span data-stu-id="c897c-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="c897c-107">在 [**外部通訊**中，選取 [**強制執行 Yammer 中的 Exchange Online Exchange 傳輸規則 (Etr)。**</span><span class="sxs-lookup"><span data-stu-id="c897c-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="c897c-108">選擇 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="c897c-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="c897c-109">如需詳細資訊，請參閱 <<c0>控制外部傳訊與 Exchange 傳輸規則的 Yammer 網路中</span><span class="sxs-lookup"><span data-stu-id="c897c-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

