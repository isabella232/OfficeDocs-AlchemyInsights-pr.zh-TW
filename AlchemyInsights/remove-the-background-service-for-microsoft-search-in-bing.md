---
title: 移除 Bing 專用 Microsoft 搜尋的背景服務
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753392"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="2becc-102">移除 Bing 專用 Microsoft 搜尋的背景服務</span><span class="sxs-lookup"><span data-stu-id="2becc-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="2becc-103">若要移除 Bing 專用 Microsoft 搜尋的背景服務，您可以嘗試下列補救方法：</span><span class="sxs-lookup"><span data-stu-id="2becc-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="2becc-104">若要還原為原始搜尋引擎設定，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="2becc-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="2becc-105">a.</span><span class="sxs-lookup"><span data-stu-id="2becc-105">a.</span></span> <span data-ttu-id="2becc-106">將 [使用 Bing 做為預設搜尋引擎]**[ 開關切換為 [關閉]](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**。</span><span class="sxs-lookup"><span data-stu-id="2becc-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="2becc-107">b.</span><span class="sxs-lookup"><span data-stu-id="2becc-107">b.</span></span> <span data-ttu-id="2becc-108">[前往 Microsoft 365 系統管理中心](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)並清除會影響組織中所有使用者的設定。</span><span class="sxs-lookup"><span data-stu-id="2becc-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="2becc-109">若要從個別裝置移除背景服務，請執行下列工作：</span><span class="sxs-lookup"><span data-stu-id="2becc-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="2becc-110">a.</span><span class="sxs-lookup"><span data-stu-id="2becc-110">a.</span></span> <span data-ttu-id="2becc-111">選擇 **[控制台] > [程式集] > [程式和功能]**。</span><span class="sxs-lookup"><span data-stu-id="2becc-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="2becc-112">b.</span><span class="sxs-lookup"><span data-stu-id="2becc-112">b.</span></span> <span data-ttu-id="2becc-113">在目前安裝程式的清單中，以滑鼠右鍵按一下 **[Bing 專用 Microsoft 搜尋]**，然後再按一下 **[解除安裝]**。</span><span class="sxs-lookup"><span data-stu-id="2becc-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="2becc-114">若要從組織中多個裝置移除背景服務，請以系統管理員身分登入，然後執行指令碼中的下列命令：</span><span class="sxs-lookup"><span data-stu-id="2becc-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
