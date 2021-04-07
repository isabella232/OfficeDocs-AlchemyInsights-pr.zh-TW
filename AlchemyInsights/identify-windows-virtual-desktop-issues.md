---
title: 識別 Windows 虛擬桌面問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590275"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="84ce9-102">識別 Windows 虛擬桌面問題</span><span class="sxs-lookup"><span data-stu-id="84ce9-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="84ce9-103">Windows 虛擬桌面診斷僅使用 PowerShell Cmdlet，但包含許多選用參數以協助縮小和隔離問題。</span><span class="sxs-lookup"><span data-stu-id="84ce9-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="84ce9-104">若要開始使用：</span><span class="sxs-lookup"><span data-stu-id="84ce9-104">To get started:</span></span> 

1. <span data-ttu-id="84ce9-105">下載並匯入 Windows 虛擬桌面 PowerShell 模組。</span><span class="sxs-lookup"><span data-stu-id="84ce9-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="84ce9-106">如需詳細資訊，請參閱[適用於 Windows PowerShell 的 Windows 虛擬桌面 Cmdlet](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)。</span><span class="sxs-lookup"><span data-stu-id="84ce9-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="84ce9-107">執行下列 Cmdlet 登入您的帳戶：</span><span class="sxs-lookup"><span data-stu-id="84ce9-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="84ce9-108">範例：`Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="84ce9-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="84ce9-109">**注意：** 所有使用 PowerShell 的査詢都必須包含 -UserName 或 -ActivityID 參數。</span><span class="sxs-lookup"><span data-stu-id="84ce9-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="84ce9-110">如需有關監視功能的資訊，請參閱使用[診斷功能的記錄分析](https://go.microsoft.com/fwlink/?linkid=2126847)。</span><span class="sxs-lookup"><span data-stu-id="84ce9-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="84ce9-111">若要依使用者篩選診斷活動，請執行以下 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="84ce9-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="84ce9-112">範例：`Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="84ce9-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="84ce9-113">您可以執行一個篩選器清單來診斷問題。</span><span class="sxs-lookup"><span data-stu-id="84ce9-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="84ce9-114">若要深入了解診斷問題，請參閱[識別和診斷 Windows 虛擬桌面問題](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)。</span><span class="sxs-lookup"><span data-stu-id="84ce9-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="84ce9-115">若要深入瞭解常見錯誤，請參閲[常見錯誤案例](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)。</span><span class="sxs-lookup"><span data-stu-id="84ce9-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
