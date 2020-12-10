---
title: 使用資料目錄變數（而非硬編碼路徑）修改 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608827"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="ffe3e-102">使用資料目錄變數（而非硬編碼路徑）修改 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ffe3e-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="ffe3e-103">例如，在 Windows 上，若要將設定檔資料儲存在使用者的本機應用程式資料下，而不是在預設位置，請將 **UserDataDir** 原則設定為 **$ {local_app_data} \Edge\Profile**。</span><span class="sxs-lookup"><span data-stu-id="ffe3e-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="ffe3e-104">若要深入瞭解，請參閱 [建立 Microsoft Edge 使用者資料目錄變數](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)。</span><span class="sxs-lookup"><span data-stu-id="ffe3e-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>