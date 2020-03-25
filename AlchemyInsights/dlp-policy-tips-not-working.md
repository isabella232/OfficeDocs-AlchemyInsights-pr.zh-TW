---
title: DLP 原則提示無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932577"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="d479f-102">DLP 原則提示問題</span><span class="sxs-lookup"><span data-stu-id="d479f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="d479f-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="d479f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d479f-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="d479f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d479f-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="d479f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d479f-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="d479f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d479f-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="d479f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d479f-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="d479f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d479f-109">**DLP 原則秘訣**</span><span class="sxs-lookup"><span data-stu-id="d479f-109">**DLP policy tips**</span></span>

<span data-ttu-id="d479f-110">使用**DLP 原則**時，使用者可能會收到與**原則提示**違規的原則提示。</span><span class="sxs-lookup"><span data-stu-id="d479f-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="d479f-111">系統管理員可以設定在測試其 DLP 原則時或當原則處於完全強制執行模式時所顯示的原則提示。</span><span class="sxs-lookup"><span data-stu-id="d479f-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="d479f-112">若要在完整執行模式中的 [安全性與合規性中心] 中設定 DLP 原則上的原則提示，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="d479f-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="d479f-113">使用[這裡](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)的步驟，確定已**啟用**DLP 規則上的原則提示。</span><span class="sxs-lookup"><span data-stu-id="d479f-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="d479f-114">確定您的**內容符合**觸發本文所述規則**所需**[的專案。](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d479f-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="d479f-115">原則提示會顯示在 OWA 和 Outlook 中。</span><span class="sxs-lookup"><span data-stu-id="d479f-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="d479f-116">不過，使用**Outlook 2013 或更新版本**時，原則秘訣只會顯示在某些情況下。</span><span class="sxs-lookup"><span data-stu-id="d479f-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="d479f-117">這些條件如下所示： [Outlook 2013 或更新版本支援的條件，以顯示原則提示](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="d479f-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="d479f-118">如需有關 DLP 原則提示的詳細資訊，請參閱：[顯示 dlp 原則的原則提示](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="d479f-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  