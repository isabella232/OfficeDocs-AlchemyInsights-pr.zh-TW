---
title: Yammer 授權問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146757"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="61212-102">Yammer 授權問題</span><span class="sxs-lookup"><span data-stu-id="61212-102">Yammer licensing issues</span></span>

<span data-ttu-id="61212-103">所有使用者都必須擁有使用 Yammer 企業版服務的授權，但根據預設，Yammer 不要求使用者需擁有存取服務的授權。</span><span class="sxs-lookup"><span data-stu-id="61212-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="61212-104">當系統管理員變更設定以封鎖沒有 Yammer 授權的 Microsoft 365 使用者時，未獲指派的 Yammer 企業版授權的使用者將無法存取 Yammer 服務。</span><span class="sxs-lookup"><span data-stu-id="61212-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="61212-105">如需詳細諮詢，請參閱 [在 Office 365 中管理 Yammer 使用者授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="61212-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="61212-106">當使用者的授權被移除時，將不再顯示 Yammer 選格，而其他服務可以使用授權移除來隱藏功能。</span><span class="sxs-lookup"><span data-stu-id="61212-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="61212-107">在其他情況下，仍然可以顯示功能，但需要授權指派才能運作。</span><span class="sxs-lookup"><span data-stu-id="61212-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="61212-108">**授權尚未為使用者更新**</span><span class="sxs-lookup"><span data-stu-id="61212-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="61212-109">有時候，儘管使用者已被指派授權，但仍無法存取 Yammer。</span><span class="sxs-lookup"><span data-stu-id="61212-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="61212-110">當有大量授權指派進行時，更有可能會發生延遲問題。</span><span class="sxs-lookup"><span data-stu-id="61212-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="61212-111">因為系統會以非同步方式執行，因此在 Azure AD 中，Yammer 使用者可能不會以變更的授權順序進行更新。</span><span class="sxs-lookup"><span data-stu-id="61212-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="61212-112">在開啟支援案例以報告授權同步處理問題之前，請等待24小時。</span><span class="sxs-lookup"><span data-stu-id="61212-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="61212-113">**大量授權指派**</span><span class="sxs-lookup"><span data-stu-id="61212-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="61212-114">您可以透過系統管理中心或 PowerShell 腳本編寫來指派授權。</span><span class="sxs-lookup"><span data-stu-id="61212-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="61212-115">如需詳細資訊，請參閱[指派授權給使用者](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)和[使用 Office 365 PowerShell 指派授權給使用者帳戶](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)。</span><span class="sxs-lookup"><span data-stu-id="61212-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="61212-116">Microsoft 支援服務不提供建立腳本的協助，但提供 Yammer 授權指派的文件。</span><span class="sxs-lookup"><span data-stu-id="61212-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="61212-117">如需詳細資訊，請參閱 [使用 Windows PowerShell 管理 Yammer 授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)。</span><span class="sxs-lookup"><span data-stu-id="61212-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>