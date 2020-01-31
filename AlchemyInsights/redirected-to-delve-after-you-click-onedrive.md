---
title: OneDrive for Business 網站 OneDrive 重新導向至 Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571190"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="6b815-102">按一下 [OneDrive] 之後，重新導向至 Delve</span><span class="sxs-lookup"><span data-stu-id="6b815-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="6b815-103">請參閱我們詳細的[疑難排解指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。</span><span class="sxs-lookup"><span data-stu-id="6b815-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="6b815-104">若要解決此問題，Office 365 系統管理員必須授與使用者建立其 「 我的網站 」 網站的權限。</span><span class="sxs-lookup"><span data-stu-id="6b815-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="6b815-105">這是因為 OneDrive for Business 頁面建立 「 我的網站。</span><span class="sxs-lookup"><span data-stu-id="6b815-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="6b815-106">若要授與此權限，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="6b815-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="6b815-107">在 SharePoint 系統管理中心中，按一下 [**使用者設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="6b815-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="6b815-108">在 [**人員**] 區段中，按一下 [**管理使用者權限**。</span><span class="sxs-lookup"><span data-stu-id="6b815-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="6b815-109">新增需要建立其 「 我的網站 」 網站的權限的使用者。</span><span class="sxs-lookup"><span data-stu-id="6b815-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="6b815-110">根據預設，此設定設為**外部使用者以外的任何人**。</span><span class="sxs-lookup"><span data-stu-id="6b815-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="6b815-111">新增使用者、 使用者或群組之後，請確定已選取 [新增的使用者、 使用者或群組，捲動至 [**權限**] 區段，然後選取 [**建立個人網站 （所需的個人存放區、 新聞摘要及追蹤內容）** 旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="6b815-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="6b815-112">按一下 [**確定**]，然後將 [瀏覽] 以建立網站的 [OneDrive] 頁面上的使用者。</span><span class="sxs-lookup"><span data-stu-id="6b815-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
