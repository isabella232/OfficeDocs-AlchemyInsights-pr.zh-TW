---
title: 有關 DLP 問題的詳細資訊
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932685"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="4a226-102">有關 DLP 問題的資訊</span><span class="sxs-lookup"><span data-stu-id="4a226-102">Information about DLP issues</span></span>

<span data-ttu-id="4a226-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="4a226-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4a226-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a226-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4a226-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="4a226-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4a226-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="4a226-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4a226-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="4a226-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4a226-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="4a226-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4a226-109">**DLP 原則的資訊**</span><span class="sxs-lookup"><span data-stu-id="4a226-109">**Information on DLP policy**</span></span>

<span data-ttu-id="4a226-110">使用 DLP 原則，您可以識別、監視和自動保護 Office 365 中的機密資訊。</span><span class="sxs-lookup"><span data-stu-id="4a226-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="4a226-111">如需詳細資訊，請流覽下列連結：</span><span class="sxs-lookup"><span data-stu-id="4a226-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="4a226-112">資料外洩防護概觀</span><span class="sxs-lookup"><span data-stu-id="4a226-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="4a226-113">機密資訊類型在找什麼</span><span class="sxs-lookup"><span data-stu-id="4a226-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="4a226-114">建立自訂機密資訊類型</span><span class="sxs-lookup"><span data-stu-id="4a226-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="4a226-115">傳送電子郵件通知並顯示原則提示</span><span class="sxs-lookup"><span data-stu-id="4a226-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="4a226-116">使用保留標籤與 DLP 來保護 SharePoint Online 檔案</span><span class="sxs-lookup"><span data-stu-id="4a226-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="4a226-117">DLP 和 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4a226-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="4a226-118">若要使用內建或自訂的機密資訊類型來測試資料，請使用 [**分類** > **機密資訊類型**] 底下的 [**測試類型**] 選項。</span><span class="sxs-lookup"><span data-stu-id="4a226-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="4a226-119">如需詳細資訊，請參閱[測試自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="4a226-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>