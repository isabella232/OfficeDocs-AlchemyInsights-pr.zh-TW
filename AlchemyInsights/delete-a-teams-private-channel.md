---
title: 刪除 Teams 私人頻道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431444"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="2dbba-102">刪除 Teams 私人頻道</span><span class="sxs-lookup"><span data-stu-id="2dbba-102">Delete a Teams private channel</span></span>

<span data-ttu-id="2dbba-103">如果您為基礎 SharePoint 網站啟用了SharePoint 保留原則，則 Microsoft 會注意到删除 Teams 私人頻道時出現的問題。</span><span class="sxs-lookup"><span data-stu-id="2dbba-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="2dbba-104">Microsoft 正在想辦法修正這個問題。</span><span class="sxs-lookup"><span data-stu-id="2dbba-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="2dbba-105">與此同時，您可以使用下列因應措施刪除私人頻道。</span><span class="sxs-lookup"><span data-stu-id="2dbba-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="2dbba-106">**從 Sharepoint 保留原則中排除小組/網站集合。**</span><span class="sxs-lookup"><span data-stu-id="2dbba-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="2dbba-107">移至 Office 365 系統管理員入口網站，然後選取左側流覽窗格中的 **[顯示所有]**。</span><span class="sxs-lookup"><span data-stu-id="2dbba-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="2dbba-108">在 **[系統管理中心]** 中，移至 \*\*[安全性與合規性] \*\* > \*\*[資料遺失防護] \*\* > \*\* [原則] \*\*。</span><span class="sxs-lookup"><span data-stu-id="2dbba-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="2dbba-109">識別任何適用於 Sharepoint 網站的原則，並修改該原則，使包含私人頻道的團隊的 Sharepoint 網站不包含在保留原則下。</span><span class="sxs-lookup"><span data-stu-id="2dbba-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="2dbba-110">儲存原則。</span><span class="sxs-lookup"><span data-stu-id="2dbba-110">Save the policy.</span></span>
    <span data-ttu-id="2dbba-111">原則設定最多可能需要 24 小時才能生效。</span><span class="sxs-lookup"><span data-stu-id="2dbba-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="2dbba-112">排除網站之後，您可以刪除私人頻道。</span><span class="sxs-lookup"><span data-stu-id="2dbba-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="2dbba-113">您***可能***可以在 Android 裝置上使用 Microsoft Teams 來刪除私人頻道。</span><span class="sxs-lookup"><span data-stu-id="2dbba-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="2dbba-114">如需相關的 SharePoint 資訊，請參閱[無法刪除 SharePoint Online 或商務用 OneDrive 中的項目](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)。</span><span class="sxs-lookup"><span data-stu-id="2dbba-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>