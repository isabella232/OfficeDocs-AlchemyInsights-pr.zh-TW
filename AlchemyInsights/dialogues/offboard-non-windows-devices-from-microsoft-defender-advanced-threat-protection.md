---
title: '從 Microsoft Defender 高級威脅防護 (的非 Windows 裝置下架 ATP) '
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529968"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="4c168-102">從 Microsoft Defender 高級威脅防護 (的非 Windows 裝置下架 ATP) </span><span class="sxs-lookup"><span data-stu-id="4c168-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="4c168-103">方法如下：</span><span class="sxs-lookup"><span data-stu-id="4c168-103">Here's how:</span></span>

1. <span data-ttu-id="4c168-104">遵循協力廠商檔，以從 Microsoft Defender ATP 中斷協力廠商解決方案的連線。</span><span class="sxs-lookup"><span data-stu-id="4c168-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="4c168-105">從您的 Azure Active Directory 租使用者移除協力廠商解決方案的許可權：</span><span class="sxs-lookup"><span data-stu-id="4c168-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="4c168-106">登入 [Azure 入口網站](https://go.microsoft.com/fwlink/?linkid=2125612)。</span><span class="sxs-lookup"><span data-stu-id="4c168-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="4c168-107">選取 [**所有服務**]  >  **Azure Active Directory**  >  **企業應用程式**。</span><span class="sxs-lookup"><span data-stu-id="4c168-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="4c168-108">選取您想要下架的應用程式。</span><span class="sxs-lookup"><span data-stu-id="4c168-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="4c168-109">選取 [刪除]。</span><span class="sxs-lookup"><span data-stu-id="4c168-109">Select **Delete**.</span></span>

<span data-ttu-id="4c168-110">若要深入瞭解，請參閱 [下架非 Windows 裝置](https://go.microsoft.com/fwlink/?linkid=2143630)。</span><span class="sxs-lookup"><span data-stu-id="4c168-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
