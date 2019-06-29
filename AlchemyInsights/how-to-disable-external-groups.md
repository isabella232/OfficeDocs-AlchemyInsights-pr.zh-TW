---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384816"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="51f6f-102">如何停用外部群組</span><span class="sxs-lookup"><span data-stu-id="51f6f-102">How to disable External Groups</span></span>

<span data-ttu-id="51f6f-103">Yammer 外部訊息套用 Exchange 傳輸規則 (ETRs), 這是一組主動控制措施, 可防止公司資訊被共用。</span><span class="sxs-lookup"><span data-stu-id="51f6f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="51f6f-104">若要限制使用者建立外部群組, 您必須設定 Exchange 傳輸規則 (ETR), 然後將 Yammer 設定為使用 Exchange 傳輸規則來封鎖外部郵件。</span><span class="sxs-lookup"><span data-stu-id="51f6f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="51f6f-105">一旦您在 Exchange Online 系統管理中心中建立規則, 請遵循下列步驟來設定 ETR 在 Yammer 中套用:</span><span class="sxs-lookup"><span data-stu-id="51f6f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="51f6f-106">以已驗證的系統管理員身分登入 Yammer, 然後在**Yammer 系統管理中心**中, 移至 [C**內容和\>安全性安全性設定]。**</span><span class="sxs-lookup"><span data-stu-id="51f6f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="51f6f-107">在 [**外部訊息**] 底下, 選取 [**在 Yammer 中強制您的 Exchange Online exchange 傳輸規則 (ETRs)]。**</span><span class="sxs-lookup"><span data-stu-id="51f6f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="51f6f-108">選擇 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="51f6f-108">Choose **Save**.</span></span>

<span data-ttu-id="51f6f-109">如需詳細資訊, 請參閱[使用 Exchange 傳輸規則控制 Yammer 網路中的外部訊息](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="51f6f-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  