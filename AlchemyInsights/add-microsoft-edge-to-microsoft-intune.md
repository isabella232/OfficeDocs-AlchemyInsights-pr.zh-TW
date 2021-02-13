---
title: 將 Microsoft Edge 新增至 Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177990"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="8c2b6-102">將 Microsoft Edge 新增至 Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8c2b6-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="8c2b6-103">若要能部署、設定、監視及保護 Windows 10 的 Microsoft Edge，您必須先將它新增至 Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="8c2b6-104">Intune 支援 Microsoft Edge 77 及更新版本。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="8c2b6-105">Intune 會偵測任何現有的 Microsoft Edge 安裝。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="8c2b6-106">如果您已在使用者的內容中安裝 Microsoft Edge，系統安裝會在使用者的內容中覆寫安裝。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="8c2b6-107">如果您已在系統內容中安裝 Microsoft Edge，將系統會報告安裝成功。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="8c2b6-108">在系統脈絡中安裝的 Microsoft Edge 會覆寫預先安裝的 Microsoft Edge 77 及更新版本 (適用于使用者脈絡中的所有通道)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="8c2b6-109">**先決條件**</span><span class="sxs-lookup"><span data-stu-id="8c2b6-109">**Prerequisite**</span></span>

<span data-ttu-id="8c2b6-110">Windows 10 版本 1709 或更新版本。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="8c2b6-111">**將 Edge 新增至 Intune 的步驟**</span><span class="sxs-lookup"><span data-stu-id="8c2b6-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="8c2b6-112">[在 Intune 中設定應用程式](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="8c2b6-113">[設定應用程式資訊](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="8c2b6-114">[設定應用程式設定](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="8c2b6-115">[選取 [範圍] 標籤 (選用)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="8c2b6-116">[新增應用程式](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="8c2b6-117">如需更多說明，請參閱 [疑難排解](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="8c2b6-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




