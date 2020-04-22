---
title: Business Web OneDrive 重新導向 Delve 的 OneDrive
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
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722801"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="6d144-102">在您按一下 OneDrive 之後重新導向 Delve</span><span class="sxs-lookup"><span data-stu-id="6d144-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="6d144-103">請參閱我們的詳細[疑難排解指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。</span><span class="sxs-lookup"><span data-stu-id="6d144-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="6d144-104">若要解決此問題，管理員必須授與使用者建立其「我的網站」網站的權利。</span><span class="sxs-lookup"><span data-stu-id="6d144-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="6d144-105">這是因為在「我的網站」上建立商務用 OneDrive 頁面。</span><span class="sxs-lookup"><span data-stu-id="6d144-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="6d144-106">若要授與此許可權，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="6d144-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="6d144-107">在 SharePoint 系統管理中心，按一下 [**使用者設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="6d144-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="6d144-108">在 [**人員**] 區段中，按一下 [**管理使用者許可權**]。</span><span class="sxs-lookup"><span data-stu-id="6d144-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="6d144-109">新增需要許可權才能建立「我的網站」網站的使用者。</span><span class="sxs-lookup"><span data-stu-id="6d144-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="6d144-110">根據預設，此設定會設定為 [**外部使用者以外的所有人**]。</span><span class="sxs-lookup"><span data-stu-id="6d144-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="6d144-111">在您新增使用者、使用者或群組之後，請確定已選取 [已新增使用者、使用者或群組]、[**許可權**] 區段，然後選取 [**建立個人網站（個人儲存區、新聞摘要和追蹤後的內容必要）**] 旁邊的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="6d144-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="6d144-112">按一下 **[確定]**，然後讓使用者流覽至 OneDrive 頁面以建立網站。</span><span class="sxs-lookup"><span data-stu-id="6d144-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
