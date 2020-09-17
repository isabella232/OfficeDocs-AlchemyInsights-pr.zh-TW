---
title: 變更預設的 Yammer 網域
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793857"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="ce8ff-102">變更預設/主要 Yammer 網域</span><span class="sxs-lookup"><span data-stu-id="ce8ff-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="ce8ff-103">Yammer URL 會包含您 Yammer 網路目前的主要網域名稱。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="ce8ff-104">此網域名稱可能與 Office 365 或 Azure AD 中設定的主要網域名稱不相符。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="ce8ff-105">新增至租用戶的自訂網域數量，以及 Yammer 是否處於受支援的組態 (1 個租用戶：1 個網路，或 1:1)，都會使行為有所差異。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="ce8ff-106">您可以取得有關 [Yammer 網域和 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) 的文件。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="ce8ff-107">存在多個 Yammer 網路且需要合併，是您看到錯誤網域最常見的原因。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="ce8ff-108">使用網路移轉工具[將資料向下整合到單一網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)是重要的第一步驟。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="ce8ff-109">請先完成此程序，然後再嘗試設定您的主要網域。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="ce8ff-110">**無自訂網域**</span><span class="sxs-lookup"><span data-stu-id="ce8ff-110">**No custom domains**</span></span>

<span data-ttu-id="ce8ff-111">針對新的租用戶，Yammer 將會使用該租用戶的預設網域 (例如 fabrikam.onmicrosoft.com)。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="ce8ff-112">主要網域會設為 yammer.com/fabrikam.onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="ce8ff-113">**單一自訂網域**</span><span class="sxs-lookup"><span data-stu-id="ce8ff-113">**Single custom domain**</span></span>

<span data-ttu-id="ce8ff-114">Yammer 會自動選取租用戶的自訂網域 (例如 fabrikam.com) 作為 Yammer 中的主要網域。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="ce8ff-115">該網域會設定為 yammer.com/fabrikam.com。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="ce8ff-116">這項變更是由網域同步服務所處理，最多可能需要 24 小時才會生效。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="ce8ff-117">**多個自訂網域**</span><span class="sxs-lookup"><span data-stu-id="ce8ff-117">**Multiple custom domains**</span></span>

<span data-ttu-id="ce8ff-118">Yammer 可以擁有與預設租用戶網域不同的主要網域。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="ce8ff-119">由於有多個自訂網域，Yammer 不會嘗試從可用網域中猜測正確網域。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="ce8ff-120">您需要開啟支援案例，要求將主要網域名稱變更為您選擇的主要網域。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="ce8ff-121">**其他疑難排解資訊**</span><span class="sxs-lookup"><span data-stu-id="ce8ff-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="ce8ff-122">在某些情況下，可能因為網域已在租用戶之間移動，因此網域同步服務無法順利執行。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="ce8ff-123">除了不正確的主要網域以外，您可能也會遇到登入或其他問題。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="ce8ff-124">若要解決此問題，您可能需要透過 Microsoft 支援服務將網域移至正確的網路。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="ce8ff-125">這種情況需要直接的協助，且可能需要一些時間來解決，特別是當您有很長的網域名稱清單時。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="ce8ff-126">開啟支援案例，以取得解決這類問題的協助。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="ce8ff-127">當您與支援專員合作時，他們會在您的控管下，檢查網域是否已在租用戶中經過驗證。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="ce8ff-128">如果新增到您租用戶的網域未經過 DNS 的驗證，他們可能會詢問關於您網域的其他驗證問題。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="ce8ff-129">請確認網域已經過 DNS 的驗證，以加快處理速度。</span><span class="sxs-lookup"><span data-stu-id="ce8ff-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
