---
title: 無法存取 Teams 聊天中共用的檔案
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505869"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="7deec-102">無法存取 Teams 聊天中共用的檔案</span><span class="sxs-lookup"><span data-stu-id="7deec-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="7deec-103">在 Microsoft Teams 中，使用者在聊天視窗中共用的檔案會自動儲存在共用使用者的 OneDrive 網站上。</span><span class="sxs-lookup"><span data-stu-id="7deec-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="7deec-104">當其他使用者嘗試在 Teams 中開啟檔案並收到「您沒有此檔案的存取權」錯誤訊息時，發生此問題的原因是您的 OneDrive 網站上已啟動「限制存取使用者」權限鎖定模式功能。</span><span class="sxs-lookup"><span data-stu-id="7deec-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="7deec-105">如需在 OneDrive 網站上停用此功能的指示，請參閱[在 Teams 中開啟檔案時發生錯誤](https://go.microsoft.com/fwlink/?linkid=2155733)。</span><span class="sxs-lookup"><span data-stu-id="7deec-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="7deec-106">檢查其他使用者是否具有 OneDrive 網站的存取權，並遵循[共用 OneDrive 檔案和資料夾](https://go.microsoft.com/fwlink/?linkid=2156017)中的指示提供存取權。</span><span class="sxs-lookup"><span data-stu-id="7deec-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>