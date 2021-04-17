---
title: Active Directory 未同步處理
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822842"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="d6b8e-102">Active Directory 未同步處理</span><span class="sxs-lookup"><span data-stu-id="d6b8e-102">Active Directory not syncing</span></span>

<span data-ttu-id="d6b8e-103">如果您收到同步處理錯誤，例如「沒有最近的同步處理」，或是注意到 Office 管理員入口網站中的目錄同步處理狀態為「上次同步處理超過3天」，可能是因為 AADConnect 的設定不正確或許可權不足，無法執行同步處理。</span><span class="sxs-lookup"><span data-stu-id="d6b8e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="d6b8e-104">使用快速設定重新安裝 AADConnect，可快速解決問題：</span><span class="sxs-lookup"><span data-stu-id="d6b8e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="d6b8e-105">[下載最新版本的 AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)。</span><span class="sxs-lookup"><span data-stu-id="d6b8e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="d6b8e-106">[依照快速安裝的指示進行](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。</span><span class="sxs-lookup"><span data-stu-id="d6b8e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="d6b8e-107">如需有關 AADConnect 服務帳戶的詳細資訊，請參閱 [Azure AD Connect：帳戶和權限](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)。</span><span class="sxs-lookup"><span data-stu-id="d6b8e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
