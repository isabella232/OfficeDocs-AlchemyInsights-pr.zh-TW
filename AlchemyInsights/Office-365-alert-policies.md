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
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 46a029f262fa05edffa6f681c7205e289fe448c5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496319"
---
# <a name="office-365-alert-policies"></a><span data-ttu-id="2ef5b-102">Office 365 警示原則</span><span class="sxs-lookup"><span data-stu-id="2ef5b-102">Office 365 Alert policies</span></span>

<span data-ttu-id="2ef5b-103">Office 365 安全性 # A0 觸發提醒具有 Office 365 企業版或 Office 365 美國政府版 E1/版 G1、 E3/G3 或 E5/G5 訂閱的組織的合規性中心提供[預設的警示原則](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-103">The Office 365 Security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="2ef5b-104">因此，系統管理員可能會收到提醒的電子郵件所傳送的通知 Office365Alerts@microsoft.com 包含主旨行例如 「 低嚴重性警示：*警示原則的名稱*」。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert:*name of alert policy*".</span></span> <span data-ttu-id="2ef5b-105">警示一般活動，例如何時會觸發警示時，會傳送通知使用者：</span><span class="sxs-lookup"><span data-stu-id="2ef5b-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="2ef5b-106">建立電子郵件轉寄的收件匣規則。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="2ef5b-107">將權限指派其信箱。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="2ef5b-108">共用，或刪除大量 SharePoint 檔案共用的檔案。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-108">Sharing or deleting a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="2ef5b-109">建立 eDiscovery 搜尋並匯出搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="2ef5b-110">若要檢閱並對警示：</span><span class="sxs-lookup"><span data-stu-id="2ef5b-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="2ef5b-111">移至[安全性 & 合規性中心](https://protection.office.com)並登入。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-111">Go to the [Security & Compliance Center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="2ef5b-112">按一下 [**提醒 > 檢視警示**。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-112">Click **Alerts > View alerts**.</span></span>
3. <span data-ttu-id="2ef5b-113">按一下 [顯示提醒的相關資訊的彈出式頁面的警示。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="2ef5b-114">您可以採取的警示，例如[移除可疑的收件匣規則](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)動作。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="2ef5b-115">或者，您只可以藉由按一下警示彈出式頁面上的 [**解決**關閉提醒。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="2ef5b-116">如需設定和管理警示原則的詳細資訊，請參閱[這篇文章](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="2ef5b-117">**重要**： 來自 Microsoft 的警示電子郵件通知絕對不會要求您執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="2ef5b-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="2ef5b-118">提供的密碼。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-118">Provide a password.</span></span>
- <span data-ttu-id="2ef5b-119">確認您的帳戶的安全性詳細資料。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-119">Verify the security details of your account.</span></span>
- <span data-ttu-id="2ef5b-120">重新驗證自己。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-120">Re-authenticate yourself.</span></span>

<span data-ttu-id="2ef5b-121">如果您收到的電子郵件就像這樣，它不由 Microsoft 所傳送，並考慮網路釣魚詐騙郵件。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="2ef5b-122">如果發生這種情況，請[將其向 Microsoft 報告](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。</span><span class="sxs-lookup"><span data-stu-id="2ef5b-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>