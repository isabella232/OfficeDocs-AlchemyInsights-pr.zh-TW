---
title: 安裝 Office 365 中的 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764901"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="02016-102">安裝 Office 365 中的 DKIM</span><span class="sxs-lookup"><span data-stu-id="02016-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="02016-103">為 Office 365 中的自訂網域設定 DKIM 的完整指示[以下](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="02016-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="02016-104">**每**個自訂網域，您需要建立**兩個**DKIM 筆 CNAME 記錄在您的網域 DNS 主機服務 （通常是網域註冊機構）。</span><span class="sxs-lookup"><span data-stu-id="02016-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="02016-105">例如，contoso.com 及 fourthcoffee.com 需要四個 DKIM CNAME 記錄： contoso.com 及 fourthcoffee.com 的兩個。</span><span class="sxs-lookup"><span data-stu-id="02016-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="02016-106">**每個**自訂網域的 DKIM CNAME 記錄使用下列格式：</span><span class="sxs-lookup"><span data-stu-id="02016-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="02016-107">**主機名稱**：`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="02016-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="02016-108">**指向位址] 或 [值**：`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="02016-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="02016-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="02016-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="02016-110">**主機名稱**：`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="02016-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="02016-111">**指向位址] 或 [值**：`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="02016-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="02016-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="02016-112">**TTL**: 3600</span></span>

   <span data-ttu-id="02016-113">\<DomainGUID\>是左邊的文字`.mail.protection.outlook.com`中自訂 MX 記錄中的自訂網域 (例如，`contoso-com`網域 contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="02016-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="02016-114">\<InitialDomain\>是您的 Office 365 (例如，contoso.onmicrosoft.com) 的註冊時所用的網域。</span><span class="sxs-lookup"><span data-stu-id="02016-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="02016-115">您已建立的 CNAME 記錄為您自訂的網域之後，請完成下列指示：</span><span class="sxs-lookup"><span data-stu-id="02016-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="02016-116">a.</span><span class="sxs-lookup"><span data-stu-id="02016-116">a.</span></span> <span data-ttu-id="02016-117">使用您的 公司或學校帳戶[登入 Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)。</span><span class="sxs-lookup"><span data-stu-id="02016-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="02016-118">b.</span><span class="sxs-lookup"><span data-stu-id="02016-118">b.</span></span> <span data-ttu-id="02016-119">選取左上角的應用程式啟動器圖示，然後選擇 [管理員]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="02016-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="02016-120">c.</span><span class="sxs-lookup"><span data-stu-id="02016-120">c.</span></span> <span data-ttu-id="02016-121">左下導覽中，依序展開 [**系統管理員**，並選擇 [ **Exchange**]。</span><span class="sxs-lookup"><span data-stu-id="02016-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="02016-122">d.</span><span class="sxs-lookup"><span data-stu-id="02016-122">d.</span></span> <span data-ttu-id="02016-123">移至 [**保護** > **DKIM**。</span><span class="sxs-lookup"><span data-stu-id="02016-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="02016-124">e.</span><span class="sxs-lookup"><span data-stu-id="02016-124">e.</span></span> <span data-ttu-id="02016-125">選取 [網域]，然後選擇**此網域的 DKIM 簽章簽署**郵件的 [**啟用**。</span><span class="sxs-lookup"><span data-stu-id="02016-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="02016-126">針對每個自訂網域重複此步驟。</span><span class="sxs-lookup"><span data-stu-id="02016-126">Repeat this step for each custom domain.</span></span>
