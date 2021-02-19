---
title: 管理外部設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282816"
---
# <a name="managing-external-settings"></a><span data-ttu-id="c580d-102">管理外部設定</span><span class="sxs-lookup"><span data-stu-id="c580d-102">Managing External Settings</span></span>

<span data-ttu-id="c580d-103">**公告**</span><span class="sxs-lookup"><span data-stu-id="c580d-103">**Announcement**</span></span>

- <span data-ttu-id="c580d-104">[從 2021年 1 月 4 日起，Google 淘汰 WebView 登入支援](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)。</span><span class="sxs-lookup"><span data-stu-id="c580d-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="c580d-105">跟隨 Google 有關測試相容性的指引，測試您的應用程式是否受到影響。</span><span class="sxs-lookup"><span data-stu-id="c580d-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="c580d-106">請確認您在使用家庭用戶 Google 帳戶登入使用者時，使用系統網頁檢視或系統瀏覽器</span><span class="sxs-lookup"><span data-stu-id="c580d-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="c580d-107">**管理邀請設定**</span><span class="sxs-lookup"><span data-stu-id="c580d-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="c580d-108">確認您已[設定 [外部共同作業設定]](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) ，以便讓適當的人員傳送邀請。</span><span class="sxs-lookup"><span data-stu-id="c580d-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="c580d-109">**管理來賓使用者存取權限**</span><span class="sxs-lookup"><span data-stu-id="c580d-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="c580d-110">通過在 [外部共同作業設定] 頁面上設定來賓存取權限，全域管理員可透過 Azure 入口網站來管理目錄中的來賓存取權限。</span><span class="sxs-lookup"><span data-stu-id="c580d-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="c580d-111">[深入了解此設定](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="c580d-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="c580d-112">如果您想要讓來賓存取 Teams 或 SharePoint 等應用程式，請確認您已設定這些應用以允許來賓存取。</span><span class="sxs-lookup"><span data-stu-id="c580d-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="c580d-113">深入了解 [Teams 設定](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) 和 [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="c580d-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c580d-114">**設定邀請：**</span><span class="sxs-lookup"><span data-stu-id="c580d-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="c580d-115">啟用 B2B 外部共同作業，並管理誰可以邀請來賓</span><span class="sxs-lookup"><span data-stu-id="c580d-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c580d-116">允許或封鎖邀請來自特定組織的使用者</span><span class="sxs-lookup"><span data-stu-id="c580d-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="c580d-117">**設定允許的身分識別提供者：**</span><span class="sxs-lookup"><span data-stu-id="c580d-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="c580d-118">Google 同盟</span><span class="sxs-lookup"><span data-stu-id="c580d-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c580d-119">直接同盟</span><span class="sxs-lookup"><span data-stu-id="c580d-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c580d-120">傳送一次性密碼驗證電子郵件</span><span class="sxs-lookup"><span data-stu-id="c580d-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
