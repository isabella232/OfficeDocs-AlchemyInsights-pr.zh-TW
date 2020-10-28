---
title: 訂閱存取
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773770"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="0475c-102">因瀏覽器問題而無法登入 Azure (瀏覽器掛起、持續旋轉、未載入等等 ) </span><span class="sxs-lookup"><span data-stu-id="0475c-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="0475c-103">您可能會因為中斷而受到影響。</span><span class="sxs-lookup"><span data-stu-id="0475c-103">You might be impacted by an outage.</span></span> <span data-ttu-id="0475c-104">請查看是否存在即時中斷： [Azure 健康狀態](https://status.azure.com/status/history/)。</span><span class="sxs-lookup"><span data-stu-id="0475c-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="0475c-105">請登出所有現用的 Azure 會話。</span><span class="sxs-lookup"><span data-stu-id="0475c-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="0475c-106">啟動網頁瀏覽器的內建或 incognito 模式。</span><span class="sxs-lookup"><span data-stu-id="0475c-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="0475c-107">您也可以嘗試重新整理瀏覽器、使用另一個瀏覽器、在上述情況下刪除快取 cookie。</span><span class="sxs-lookup"><span data-stu-id="0475c-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="0475c-108">深入瞭解： [疑難排解登錄問題](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="0475c-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="0475c-109">**無法存取訂閱**</span><span class="sxs-lookup"><span data-stu-id="0475c-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="0475c-110">在 [Azure 入口網站](https://portal.azure.com/)中，確定已從右上方的帳戶選取正確的 Azure 目錄。</span><span class="sxs-lookup"><span data-stu-id="0475c-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="0475c-111">在 [Azure 帳戶中心](https://account.windowsazure.com/Subscriptions)，確定所使用的帳戶是否為帳戶管理員。</span><span class="sxs-lookup"><span data-stu-id="0475c-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="0475c-112">深入瞭解： [疑難排解未找到訂閱](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="0475c-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="0475c-113">**無法存取帳單記錄**</span><span class="sxs-lookup"><span data-stu-id="0475c-113">**Unable to access billing history**</span></span>

<span data-ttu-id="0475c-114">帳戶管理員必須確定存取計費資訊的使用者已新增至 Azure Active directory，以作為來賓使用者：新增 [或刪除新使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="0475c-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0475c-115">然後，使用者必須具有全域系統管理員角色： [將角色指派給使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="0475c-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0475c-116">張貼此專案時，使用者可以使用 RBAC 原則授與存取權： [授與帳單的存取權](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="0475c-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0475c-117">**建譯的文件**</span><span class="sxs-lookup"><span data-stu-id="0475c-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="0475c-118">我無法登入以管理我的 Azure 訂閱</span><span class="sxs-lookup"><span data-stu-id="0475c-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)