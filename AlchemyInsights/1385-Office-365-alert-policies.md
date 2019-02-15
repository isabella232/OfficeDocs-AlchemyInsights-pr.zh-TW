---
title: 1385-office-365-警示-原則
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: a0a1c749a120714c33cffd9fbdad08ea2cd6d62f
ms.sourcegitcommit: 983d08cd9ffe9542db75102b5b5c036d38eff67b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/14/2019
ms.locfileid: "30056675"
---
# <a name="office-365-alert-policies"></a><span data-ttu-id="f1373-102">Office 365 警示原則</span><span class="sxs-lookup"><span data-stu-id="f1373-102">Office 365 Alert policies</span></span>

<span data-ttu-id="f1373-p101">Office 365 安全性 & 規範中心提供[預設警示原則](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)觸發組織與 Office 365 Enterprise 或 Office 365 美國政府 E1/G1、 E3/G3 或 E5/G5 訂閱的提醒。因此，系統管理員可能會收到提醒的電子郵件所傳送的通知 Office365Alerts@microsoft.com 包含主旨行例如"為低嚴重性通知：*警示原則的名稱*"。提醒時的一般活動的時觸發提醒傳送通知使用者：</span><span class="sxs-lookup"><span data-stu-id="f1373-p101">The Office 365 Security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription. Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert:*name of alert policy*". Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="f1373-106">建立將電子郵件轉寄的收件匣規則。</span><span class="sxs-lookup"><span data-stu-id="f1373-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="f1373-107">指派權限他們的信箱。</span><span class="sxs-lookup"><span data-stu-id="f1373-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="f1373-108">共用或刪除 SharePoint 檔案共用的檔案的數目。</span><span class="sxs-lookup"><span data-stu-id="f1373-108">Sharing or deleting a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="f1373-109">建立 eDiscovery 搜尋和匯出搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="f1373-109">Create eDiscovery searches and export search results.</span></span>
 
<span data-ttu-id="f1373-110">若要檢閱並處理通知：</span><span class="sxs-lookup"><span data-stu-id="f1373-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="f1373-111">移至 [[安全性 & 規範中心](https://protection.office.com)並登入。</span><span class="sxs-lookup"><span data-stu-id="f1373-111">Go to the [Security & Compliance Center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="f1373-112">按一下 [**提醒 > 檢視提醒**。</span><span class="sxs-lookup"><span data-stu-id="f1373-112">Click **Alerts > View alerts**.</span></span>
3. <span data-ttu-id="f1373-113">按一下 [顯示提醒的相關資訊與彈出式] 頁面上的提醒。</span><span class="sxs-lookup"><span data-stu-id="f1373-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="f1373-p102">您可以採取通知，例如[移除可疑的收件匣規則](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)動作。或您只可以關閉此通知警示彈出式] 頁面上按一下 [**解析**。</span><span class="sxs-lookup"><span data-stu-id="f1373-p102">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account). Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="f1373-116">如需設定及管理警示原則的詳細資訊，請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="f1373-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="f1373-117">**重要**： 使用 microsoft 的提醒的電子郵件通知絕對不會要求您可以執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="f1373-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="f1373-118">提供密碼。</span><span class="sxs-lookup"><span data-stu-id="f1373-118">Provide a password.</span></span>
- <span data-ttu-id="f1373-119">確認您的帳戶安全性的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="f1373-119">Verify the security details of your account.</span></span>
- <span data-ttu-id="f1373-120">重新驗證自己。</span><span class="sxs-lookup"><span data-stu-id="f1373-120">Re-authenticate yourself.</span></span>

<span data-ttu-id="f1373-p103">如果您收到電子郵件訊息類似，它不會傳送由 Microsoft 和應考慮使用網路釣魚詐騙郵件。如果發生的問題，請[將其向 Microsoft 報告](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。</span><span class="sxs-lookup"><span data-stu-id="f1373-p103">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam. If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>