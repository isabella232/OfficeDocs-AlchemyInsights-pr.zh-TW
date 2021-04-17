---
title: Teams 允許或停用 IP 視訊
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826334"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="36f49-102">Teams 允許或停用 IP 視訊</span><span class="sxs-lookup"><span data-stu-id="36f49-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="36f49-103">**變更或建立會議原則**</span><span class="sxs-lookup"><span data-stu-id="36f49-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="36f49-104">若要變更或建立會議原則，請移至 [Microsoft Teams 系統管理中心] > [會議] > [會議原則 **]**。</span><span class="sxs-lookup"><span data-stu-id="36f49-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="36f49-105">從清單中選取原則，或按一下 [新增]。</span><span class="sxs-lookup"><span data-stu-id="36f49-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="36f49-106">如果您要建立新原則，請新增原則的名稱和描述。</span><span class="sxs-lookup"><span data-stu-id="36f49-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="36f49-107">名稱不能包含特殊字元，且長度不可超過 64 個字元。</span><span class="sxs-lookup"><span data-stu-id="36f49-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="36f49-108">選擇您的設定，然後按一下 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="36f49-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="36f49-109">例如，假設您有許多使用者，並且想要限制其會議所需的頻寬量。</span><span class="sxs-lookup"><span data-stu-id="36f49-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="36f49-110">您可以建立名為「有限頻寬」的新自訂原則，並停用下列設定：</span><span class="sxs-lookup"><span data-stu-id="36f49-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="36f49-111">在 [音訊與視訊] 下：</span><span class="sxs-lookup"><span data-stu-id="36f49-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="36f49-112">關閉 [允許雲端錄製]。</span><span class="sxs-lookup"><span data-stu-id="36f49-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="36f49-113">關閉 [允許 IP 視訊]。</span><span class="sxs-lookup"><span data-stu-id="36f49-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="36f49-114">然後，將原則指派給使用者。</span><span class="sxs-lookup"><span data-stu-id="36f49-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="36f49-115">**將會議原則指派給使用者**</span><span class="sxs-lookup"><span data-stu-id="36f49-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="36f49-116">在 Microsoft Teams 系統管理中心的左側瀏覽窗格中，移至 [使用者]，然後按一下該使用者。</span><span class="sxs-lookup"><span data-stu-id="36f49-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="36f49-117">按一下使用者名稱左方以選取使用者，然後按一下 [編輯設定]。</span><span class="sxs-lookup"><span data-stu-id="36f49-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="36f49-118">在 [會議原則 **]** 下，選取要指派的原則，然後按一下 [套用 **]**。</span><span class="sxs-lookup"><span data-stu-id="36f49-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="36f49-119">如需詳細資訊，請參閱[在 Teams 中管理會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="36f49-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
