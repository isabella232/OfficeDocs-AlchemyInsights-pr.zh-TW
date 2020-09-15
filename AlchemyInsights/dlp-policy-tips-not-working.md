---
title: DLP 原則提示無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679576"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="bfef9-102">DLP 原則提示問題</span><span class="sxs-lookup"><span data-stu-id="bfef9-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="bfef9-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="bfef9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="bfef9-104">**DLP 原則秘訣**</span><span class="sxs-lookup"><span data-stu-id="bfef9-104">**DLP policy tips**</span></span>

<span data-ttu-id="bfef9-105">使用 **DLP 原則**時，使用者可能會收到與 **原則提示**違規的原則提示。</span><span class="sxs-lookup"><span data-stu-id="bfef9-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="bfef9-106">系統管理員可以設定在測試其 DLP 原則時或當原則處於完全強制執行模式時所顯示的原則提示。</span><span class="sxs-lookup"><span data-stu-id="bfef9-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="bfef9-107">若要在完整執行模式中的 [安全性與合規性中心] 中設定 DLP 原則上的原則提示，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="bfef9-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="bfef9-108">使用[這裡](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)的步驟，確定已**啟用**DLP 規則上的原則提示。</span><span class="sxs-lookup"><span data-stu-id="bfef9-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="bfef9-109">確定您的**內容符合**觸發本文所述規則**所需**[的專案。](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="bfef9-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="bfef9-110">原則提示會顯示在 OWA 和 Outlook 中。</span><span class="sxs-lookup"><span data-stu-id="bfef9-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="bfef9-111">不過，使用 **Outlook 2013 或更新版本**時，原則秘訣只會顯示在某些情況下。</span><span class="sxs-lookup"><span data-stu-id="bfef9-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="bfef9-112">這些條件如下所示： [Outlook 2013 或更新版本支援的條件，以顯示原則提示](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="bfef9-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="bfef9-113">如需有關 DLP 原則提示的詳細資訊，請參閱： [顯示 dlp 原則的原則提示](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="bfef9-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  