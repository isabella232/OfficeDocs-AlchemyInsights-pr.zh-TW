---
title: 權限繼承
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 791085593433dcad9b800fdea8c7ea4a878604e7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581042"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="ba9a6-102">許可權繼承在 SharePoint 中的運作方式</span><span class="sxs-lookup"><span data-stu-id="ba9a6-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="ba9a6-103">根據預設，SharePoint 中的許可權會從階層中較高的位置繼承。</span><span class="sxs-lookup"><span data-stu-id="ba9a6-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="ba9a6-104">因此，檔案會從該資料夾繼承其許可權，該資料夾繼承來自此程式庫的許可權，而該網站會從網站集合繼承其許可權。</span><span class="sxs-lookup"><span data-stu-id="ba9a6-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="ba9a6-105">如需移除唯一許可權及還原繼承的資訊，請參閱[編輯和管理清單或文件庫的許可權](https://go.microsoft.com/fwlink/?linkid=869946)。</span><span class="sxs-lookup"><span data-stu-id="ba9a6-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

