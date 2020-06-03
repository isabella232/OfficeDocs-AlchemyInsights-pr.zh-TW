---
title: DLP 未如期運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507469"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="adc3e-102">DLP 未如期運作</span><span class="sxs-lookup"><span data-stu-id="adc3e-102">DLP not working as expected</span></span>

<span data-ttu-id="adc3e-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="adc3e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="adc3e-104">**設定 DLP**</span><span class="sxs-lookup"><span data-stu-id="adc3e-104">**Setting up DLP**</span></span>

<span data-ttu-id="adc3e-105">Office 365 中的**資料遺失防護（DLP）** 未如期運作時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="adc3e-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="adc3e-106">如果是的話，請確定已正確設定**dlp 原則**，且您的資料包含**dlp 原則**在評估時所要尋找的專案。</span><span class="sxs-lookup"><span data-stu-id="adc3e-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="adc3e-107">DLP 原則可讓您識別及保護組織中的機密資訊。</span><span class="sxs-lookup"><span data-stu-id="adc3e-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="adc3e-108">若要設定 DLP 原則，請在[這裡](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)使用資訊。</span><span class="sxs-lookup"><span data-stu-id="adc3e-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="adc3e-109">**DLP 原則的查找範圍**</span><span class="sxs-lookup"><span data-stu-id="adc3e-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="adc3e-110">在安全性與合規性中心使用內**建的敏感資訊類型**時，當偵測到這些敏感類型時，DLP 原則會尋找特定的模式和元素。</span><span class="sxs-lookup"><span data-stu-id="adc3e-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="adc3e-111">**內建的敏感資訊類型**</span><span class="sxs-lookup"><span data-stu-id="adc3e-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="adc3e-112">如需有關內建機密類型和 DLP 原則在偵測敏感類型時所尋找的資訊，請參閱：[敏感資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。</span><span class="sxs-lookup"><span data-stu-id="adc3e-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="adc3e-113">**自訂敏感資訊類型**</span><span class="sxs-lookup"><span data-stu-id="adc3e-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="adc3e-114">如果您嘗試建立自訂的機密資訊類型，請使用下列文章，以取得如何建立自訂機密資訊類型的詳細資訊：[建立自訂的機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="adc3e-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="adc3e-115">**測試 DLP 原則**</span><span class="sxs-lookup"><span data-stu-id="adc3e-115">**Test a DLP policy**</span></span>

<span data-ttu-id="adc3e-116">若要使用內建或自訂的機密資訊類型來測試資料，請使用 [**分類** **Test type**  >  **機密資訊類型**] 底下的 [測試類型] 選項。</span><span class="sxs-lookup"><span data-stu-id="adc3e-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="adc3e-117">如需詳細資訊，請參閱[測試自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="adc3e-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="adc3e-118">**報告**</span><span class="sxs-lookup"><span data-stu-id="adc3e-118">**Reports**</span></span>
  
- <span data-ttu-id="adc3e-119">使用[DLP 報告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。</span><span class="sxs-lookup"><span data-stu-id="adc3e-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="adc3e-120">請參閱事件的特定詳細資料與[附隨報告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)。</span><span class="sxs-lookup"><span data-stu-id="adc3e-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
