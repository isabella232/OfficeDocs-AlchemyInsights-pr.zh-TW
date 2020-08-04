---
title: 設定端點 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "46543756"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="30a3b-102">設定端點 DLP</span><span class="sxs-lookup"><span data-stu-id="30a3b-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="30a3b-103">Microsoft 端點 DLP 可讓可以您將 DLP 保護和監視功能延伸到 Windows 10 裝置上的敏感性資訊。</span><span class="sxs-lookup"><span data-stu-id="30a3b-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="30a3b-104">將裝置上線至裝置管理中後，您就可以建立 DLP 原則，在項目上強制執行保護動作。</span><span class="sxs-lookup"><span data-stu-id="30a3b-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="30a3b-105">活動總管可用來監視敏感性項目的活動。</span><span class="sxs-lookup"><span data-stu-id="30a3b-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="30a3b-106">如需詳細資訊，請參閱 [將裝置上線至裝置管理](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="30a3b-107">若要開始使用端點 DLP：</span><span class="sxs-lookup"><span data-stu-id="30a3b-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="30a3b-108">請確認您擁有適當的 SKU/訂閱授權。</span><span class="sxs-lookup"><span data-stu-id="30a3b-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="30a3b-109">如需詳細資訊，請參閱 [SKU/訂閱授權](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="30a3b-110">檢查啟用裝置管理、存取上線頁面或開啟/關閉裝置監視所需的權限。</span><span class="sxs-lookup"><span data-stu-id="30a3b-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="30a3b-111">如需詳細資訊，請參閱 [權限](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="30a3b-112">遵循上線裝置程序將裝置上線至裝置管理。</span><span class="sxs-lookup"><span data-stu-id="30a3b-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="30a3b-113">如果您在 M365 合規性 **設定** 下方找不到 [裝置上線] (預覽) 選項，請確認您擁有上述的適當授權和權限。</span><span class="sxs-lookup"><span data-stu-id="30a3b-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="30a3b-114">如需詳細資訊，請參閱 [上線裝置](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="30a3b-115">建立 DLP 原則以保護您的敏感性項目。</span><span class="sxs-lookup"><span data-stu-id="30a3b-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="30a3b-116">如需詳細資訊，請參閱 [端點 DLP 原則案例](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="30a3b-117">如需有關 Microsoft 端點 DLP，請參閱 [深入了解 Microsoft 365 端點資料外洩防護 (預覽版)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)。</span><span class="sxs-lookup"><span data-stu-id="30a3b-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>