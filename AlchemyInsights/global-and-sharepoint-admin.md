---
title: 全域和 SharePoint 系統管理員
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002962"
- "5674"
ms.openlocfilehash: 9d4c5da8b6dc78aa18fd29589495b77b7d835aba
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706366"
---
# <a name="global-and-sharepoint-admin"></a><span data-ttu-id="50afa-102">全域和 SharePoint 系統管理員</span><span class="sxs-lookup"><span data-stu-id="50afa-102">Global and SharePoint admin</span></span>

<span data-ttu-id="50afa-103">您必須將 SharePoint 授權指派給全域和 SharePoint 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="50afa-103">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="50afa-104">剛使用 SharePoint 授權或系統管理員角色指派的新建帳戶，可能會在存取 SharePoint 時遇到問題，例如「拒絕存取」或「找不到使用者」。</span><span class="sxs-lookup"><span data-stu-id="50afa-104">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="50afa-105">請至少等候 24 小時，以完成整個系統的同步處理。</span><span class="sxs-lookup"><span data-stu-id="50afa-105">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="50afa-106">我們知道 24 小時可能感覺有點久。</span><span class="sxs-lookup"><span data-stu-id="50afa-106">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="50afa-107">多數情況下，我們已經著手研究解決方案。</span><span class="sxs-lookup"><span data-stu-id="50afa-107">In many cases, we're already working on a solution.</span></span>

<span data-ttu-id="50afa-108">獲派全域或 SharePoint 系統管理員角色的使用者可以存取 SharePoint 系統管理中心，還可以建立及管理網站 (之前稱為「網站集合」)、指定網站系統管理員、管理共用設定等。</span><span class="sxs-lookup"><span data-stu-id="50afa-108">Users assigned the Global or SharePoint admin role have access to the SharePoint admin center and can create and manage sites (previously called "site collections"), designate site admins, manage sharing settings, and more.</span></span> <span data-ttu-id="50afa-109">他們無法自動存取所有網站和每個使用者的 OneDrive，但他們可以授與自己權限，來存取存取任何網站或 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="50afa-109">They don't have automatic access to all sites and each user's OneDrive, but they can give themselves access to any site or OneDrive.</span></span> <span data-ttu-id="50afa-110">他們也可以使用 Microsoft PowerShell 來管理 SharePoint 和 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="50afa-110">They can also use Microsoft PowerShell to manage SharePoint and OneDrive.</span></span>

<span data-ttu-id="50afa-111">若要深入了解，請參閱[關於 Microsoft 365 中的 SharePoint 系統管理員角色](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)。</span><span class="sxs-lookup"><span data-stu-id="50afa-111">To learn more, see [About the SharePoint admin role in Microsoft 365](https://docs.microsoft.com/sharepoint/sharepoint-admin-role).</span></span>
<span data-ttu-id="50afa-112">Microsoft SharePoint 或 Microsoft OneDrive 變成無法存取的原因可能有數個。</span><span class="sxs-lookup"><span data-stu-id="50afa-112">There are several reasons why Microsoft SharePoint or Microsoft OneDrive might become inaccessible.</span></span> <span data-ttu-id="50afa-113">如果您無法存取 SharePoint Online，請使用下列指南來解決此問題。</span><span class="sxs-lookup"><span data-stu-id="50afa-113">If you can't access SharePoint Online, use the following guide to troubleshoot this issue.</span></span>

- [<span data-ttu-id="50afa-114">無法存取 SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="50afa-114">Unable to access SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [<span data-ttu-id="50afa-115">SharePoint 或 OneDrive 系統管理中心中受 PIM 管理的使用者帳戶遭到拒絕存取</span><span class="sxs-lookup"><span data-stu-id="50afa-115">Access denied for PIM-managed user accounts in SharePoint or OneDrive admin center</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)