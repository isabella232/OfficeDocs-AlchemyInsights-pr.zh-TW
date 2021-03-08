---
title: 停止郵件自動移至封存
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
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522365"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="79077-102">停止郵件自動移至封存</span><span class="sxs-lookup"><span data-stu-id="79077-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="79077-103">如果您是使用保留原則，您可以變更該原則中的保留天數，以停止自動封存郵件。</span><span class="sxs-lookup"><span data-stu-id="79077-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="79077-104">方法如下：</span><span class="sxs-lookup"><span data-stu-id="79077-104">Here's how:</span></span>

1. <span data-ttu-id="79077-105">在 [Exchange 系統管理中心](https://go.microsoft.com/fwlink/?linkid=2059104)中，選擇 [**規範管理**] [  >  **保留標記**]。</span><span class="sxs-lookup"><span data-stu-id="79077-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="79077-106">找到 [移至封存] 保留標記。</span><span class="sxs-lookup"><span data-stu-id="79077-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="79077-107">在 [保留標記] 中，將 [保留期間 (封存期間) 變更為 [ **永不** 停用保留原則自動封存專案]。</span><span class="sxs-lookup"><span data-stu-id="79077-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="79077-108">這會變更所有已套用此保留標記之信箱的封存設定。</span><span class="sxs-lookup"><span data-stu-id="79077-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
