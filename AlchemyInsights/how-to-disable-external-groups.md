---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278457"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d4007-102">如何停用外部群組</span><span class="sxs-lookup"><span data-stu-id="d4007-102">How to disable External Groups</span></span>

<span data-ttu-id="d4007-p101">Yammer 外部通訊適用於 Exchange 傳輸規則 (ETRs) 一組主動式控制項來防止公司資訊共用。若要限制使用者，建立外部群組，您需要設定對 Exchange 傳輸規則 (ETR)，然後再設定要使用 Exchange 傳輸規則封鎖外部通訊的 Yammer。</span><span class="sxs-lookup"><span data-stu-id="d4007-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="d4007-105">一旦您已在 Exchange Online 系統管理中心內建立規則，請遵循下列步驟設定要套用的 Yammer ETR：</span><span class="sxs-lookup"><span data-stu-id="d4007-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d4007-106">登入 Yammer 身為已驗證的管理員，並在**Yammer 系統管理中心**，移至 C **ontent 與安全性\>安全性設定。**</span><span class="sxs-lookup"><span data-stu-id="d4007-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="d4007-107">在 [**外部通訊**] 下選取**Yammer 中強制執行您 Exchange Online Exchange 傳輸規則 (ETRs)。**</span><span class="sxs-lookup"><span data-stu-id="d4007-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="d4007-108">選擇 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="d4007-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="d4007-109">如需詳細資訊，請參閱[外部通訊與 Exchange 傳輸規則的 Yammer 網路中的控制項](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="d4007-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

