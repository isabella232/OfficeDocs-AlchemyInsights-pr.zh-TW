---
title: '疑難排解語音信箱 '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607997"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="90aec-102">疑難排解語音信箱</span><span class="sxs-lookup"><span data-stu-id="90aec-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="90aec-103">確定「忙碌忙碌」功能是有意的功能。</span><span class="sxs-lookup"><span data-stu-id="90aec-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="90aec-104">若此使用者不需要此功能：</span><span class="sxs-lookup"><span data-stu-id="90aec-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="90aec-105">前往 [小組系統管理中心](https://admin.teams.microsoft.com/policies/calling)。</span><span class="sxs-lookup"><span data-stu-id="90aec-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="90aec-106">在左滑軌上，流覽 **語音**  >  **通話原則**  >  **管理\*\*\*\*通話原則** 上的原則。</span><span class="sxs-lookup"><span data-stu-id="90aec-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="90aec-107">選取 [ **管理使用者**]。</span><span class="sxs-lookup"><span data-stu-id="90aec-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="90aec-108">**在呼叫** **Off** 時，搜尋使用者並將呼叫原則變更為已忙碌繁忙的呼叫原則。</span><span class="sxs-lookup"><span data-stu-id="90aec-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="90aec-109">按一下 **[套用]**。</span><span class="sxs-lookup"><span data-stu-id="90aec-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="90aec-110">對原則所做的變更最多可能需要24小時才能進行複製。</span><span class="sxs-lookup"><span data-stu-id="90aec-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="90aec-111">如需此功能的詳細資訊，請參閱： [通話時可使用忙碌的繁忙狀態](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)。</span><span class="sxs-lookup"><span data-stu-id="90aec-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
