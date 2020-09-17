---
title: 安裝 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808698"
---
# <a name="setup-dkim"></a><span data-ttu-id="4d4ea-102">安裝 DKIM</span><span class="sxs-lookup"><span data-stu-id="4d4ea-102">Setup DKIM</span></span>

<span data-ttu-id="4d4ea-103">在 Microsoft [365 的自](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)定義網域設定 DKIM 的完整指示如下。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="4d4ea-104">針對 **每個** 自訂網域，您必須在網域的 DNS 主機服務上建立 **兩個** DKIM CNAME 記錄：網域註冊機構)  (一般。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4d4ea-105">例如，contoso.com 和 fourthcoffee.com 需要四個 DKIM CNAME 記錄：兩個用於 contoso.com，而兩個用於 fourthcoffee.com。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4d4ea-106">**每個**自訂網域的 DKIM CNAME 記錄使用下列格式：</span><span class="sxs-lookup"><span data-stu-id="4d4ea-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4d4ea-107">**主機名稱**： `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4d4ea-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4d4ea-108">**指向 address 或 value**： `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4d4ea-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4d4ea-109">**TTL**：3600</span><span class="sxs-lookup"><span data-stu-id="4d4ea-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4d4ea-110">**主機名稱**： `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4d4ea-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4d4ea-111">**指向 address 或 value**： `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4d4ea-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4d4ea-112">**TTL**：3600</span><span class="sxs-lookup"><span data-stu-id="4d4ea-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4d4ea-113">\<DomainGUID\> 是 `.mail.protection.outlook.com` 自訂網域之自訂 MX 記錄中的文字 (例如， `contoso-com` 針對 domain contoso.com) 。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4d4ea-114">\<InitialDomain\> 是您註冊 Microsoft 365 時所使用的網域 (例如，contoso.onmicrosoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4d4ea-115">在您為自訂網域建立 CNAME 記錄後，請完成下列指示：</span><span class="sxs-lookup"><span data-stu-id="4d4ea-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4d4ea-116">a.</span><span class="sxs-lookup"><span data-stu-id="4d4ea-116">a.</span></span> <span data-ttu-id="4d4ea-117">使用您的公司或學校帳戶登[入 Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4d4ea-118">b.</span><span class="sxs-lookup"><span data-stu-id="4d4ea-118">b.</span></span> <span data-ttu-id="4d4ea-119">選取左上角的應用程式啟動器圖示，然後選擇 [管理員]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4d4ea-120">c.</span><span class="sxs-lookup"><span data-stu-id="4d4ea-120">c.</span></span> <span data-ttu-id="4d4ea-121">在導覽的左下角展開 [管理員]\*\*\*\*，然後選擇 [Exchange]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4d4ea-122">d.</span><span class="sxs-lookup"><span data-stu-id="4d4ea-122">d.</span></span> <span data-ttu-id="4d4ea-123">移至 [**保護**  >  **DKIM**]。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4d4ea-124">e.</span><span class="sxs-lookup"><span data-stu-id="4d4ea-124">e.</span></span> <span data-ttu-id="4d4ea-125">選取 [網域]，然後選擇 [**啟用\*\*\*\*此網域的簽署郵件] 與 DKIM 的特徵碼**。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4d4ea-126">對每個自訂網域重複此步驟。</span><span class="sxs-lookup"><span data-stu-id="4d4ea-126">Repeat this step for each custom domain.</span></span>
