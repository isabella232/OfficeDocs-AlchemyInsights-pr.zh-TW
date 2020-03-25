---
title: DLP 未如期運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932613"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="af27e-102">DLP 未如期運作</span><span class="sxs-lookup"><span data-stu-id="af27e-102">DLP not working as expected</span></span>

<span data-ttu-id="af27e-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="af27e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="af27e-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="af27e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="af27e-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="af27e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="af27e-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="af27e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="af27e-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="af27e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="af27e-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="af27e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="af27e-109">**設定 DLP**</span><span class="sxs-lookup"><span data-stu-id="af27e-109">**Setting up DLP**</span></span>

<span data-ttu-id="af27e-110">Office 365 中的**資料遺失防護（DLP）** 未如期運作時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="af27e-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="af27e-111">如果是的話，請確定已正確設定**dlp 原則**，且您的資料包含**dlp 原則**在評估時所要尋找的專案。</span><span class="sxs-lookup"><span data-stu-id="af27e-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="af27e-112">DLP 原則可讓您識別及保護組織中的機密資訊。</span><span class="sxs-lookup"><span data-stu-id="af27e-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="af27e-113">若要設定 DLP 原則，請在[這裡](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)使用資訊。</span><span class="sxs-lookup"><span data-stu-id="af27e-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="af27e-114">**DLP 原則的查找範圍**</span><span class="sxs-lookup"><span data-stu-id="af27e-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="af27e-115">在 Office 365 安全性與合規性中心使用內**建的敏感資訊類型**時，當偵測到這些敏感類型時，DLP 原則會尋找特定的模式和元素。</span><span class="sxs-lookup"><span data-stu-id="af27e-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="af27e-116">**內建的敏感資訊類型**</span><span class="sxs-lookup"><span data-stu-id="af27e-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="af27e-117">如需有關內建機密類型和 DLP 原則在偵測敏感類型時所尋找的資訊，請參閱：[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="af27e-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="af27e-118">**自訂敏感資訊類型**</span><span class="sxs-lookup"><span data-stu-id="af27e-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="af27e-119">如果您嘗試建立自訂的機密資訊類型，請使用下列文章，以取得如何建立自訂機密資訊類型的詳細資訊：[建立自訂的機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="af27e-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="af27e-120">**測試 DLP 原則**</span><span class="sxs-lookup"><span data-stu-id="af27e-120">**Test a DLP policy**</span></span>

<span data-ttu-id="af27e-121">若要使用內建或自訂的機密資訊類型來測試資料，請使用 [**分類** > **機密資訊類型**] 底下的 [**測試類型**] 選項。</span><span class="sxs-lookup"><span data-stu-id="af27e-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="af27e-122">如需詳細資訊，請參閱[測試自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="af27e-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="af27e-123">**報告**</span><span class="sxs-lookup"><span data-stu-id="af27e-123">**Reports**</span></span>
  
- <span data-ttu-id="af27e-124">使用[DLP 報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。</span><span class="sxs-lookup"><span data-stu-id="af27e-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="af27e-125">請參閱事件的特定詳細資料與[附隨報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)。</span><span class="sxs-lookup"><span data-stu-id="af27e-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
