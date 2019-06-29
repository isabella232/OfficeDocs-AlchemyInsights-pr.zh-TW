---
title: DLP 未如預期運作
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
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389604"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="755ea-102">DLP 未如預期運作</span><span class="sxs-lookup"><span data-stu-id="755ea-102">DLP not working as expected</span></span>

<span data-ttu-id="755ea-103">您是否遇到 Office 365 中**資料遺失防護 (DLP)** 的問題無法如預期般運作？</span><span class="sxs-lookup"><span data-stu-id="755ea-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="755ea-104">如果是的話, 請確定您的**DLP 原則**設定正確, 且您的資料包含了**dlp 原則**在評估時所要尋找的內容。</span><span class="sxs-lookup"><span data-stu-id="755ea-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="755ea-105">**設定 DLP:**</span><span class="sxs-lookup"><span data-stu-id="755ea-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="755ea-106">DLP 原則可讓您識別和保護組織中的敏感資訊。</span><span class="sxs-lookup"><span data-stu-id="755ea-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="755ea-107">若要設定 DLP 原則, 請使用[此處](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的資訊。</span><span class="sxs-lookup"><span data-stu-id="755ea-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="755ea-108">**DLP 原則尋找的內容:**</span><span class="sxs-lookup"><span data-stu-id="755ea-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="755ea-109">在 Office 365 安全性與合規性中心使用**內建的機密資訊類型**時, DLP 原則會在偵測這些敏感類型時, 尋找特定模式和元素。</span><span class="sxs-lookup"><span data-stu-id="755ea-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="755ea-110">**內建的機密資訊類型:**</span><span class="sxs-lookup"><span data-stu-id="755ea-110">**Built-in Sensitive Information Types:**</span></span>

    <span data-ttu-id="755ea-111">如需內建敏感類型以及偵測敏感類型時 DLP 原則所尋找的詳細資訊, 請參閱:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="755ea-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="755ea-112">**自訂機密資訊類型:**</span><span class="sxs-lookup"><span data-stu-id="755ea-112">**Custom Sensitive Information Types:**</span></span>

    <span data-ttu-id="755ea-113">如果您嘗試建立自訂的機密資訊類型, 請使用下列文章, 以取得如何建立自訂機密資訊類型的資訊:[建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="755ea-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

 <span data-ttu-id="755ea-114">**下屬**</span><span class="sxs-lookup"><span data-stu-id="755ea-114">**Reports:**</span></span>
  
- <span data-ttu-id="755ea-115">使用[DLP 報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。</span><span class="sxs-lookup"><span data-stu-id="755ea-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="755ea-116">請參閱事件的特定詳細資料與[附隨報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)。</span><span class="sxs-lookup"><span data-stu-id="755ea-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
