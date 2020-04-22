---
title: 1385-Office-365-警示-原則
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 1209e59668bbe69fe88408933ae11b357b8d4f1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687609"
---
# <a name="alert-policies"></a><span data-ttu-id="99e9d-102">警示原則</span><span class="sxs-lookup"><span data-stu-id="99e9d-102">Alert policies</span></span>

<span data-ttu-id="99e9d-103">Microsoft 365 security & 合規性中心提供[預設的警示原則](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)，可觸發 Office 365 企業版或 OFFICE 365 US 政府 E1/G1、E3/G3 或 E5/G5 訂閱的組織警示。</span><span class="sxs-lookup"><span data-stu-id="99e9d-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="99e9d-104">因此，系統管理員可能會收到 Office365Alerts@microsoft.com 使用主旨列（如「嚴重性警示：*警示原則的名稱*」）傳送的警示電子郵件通知。</span><span class="sxs-lookup"><span data-stu-id="99e9d-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="99e9d-105">當一般活動（例如使用者）觸發警示時，會傳送警示通知。</span><span class="sxs-lookup"><span data-stu-id="99e9d-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="99e9d-106">建立轉寄電子郵件的收件匣規則。</span><span class="sxs-lookup"><span data-stu-id="99e9d-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="99e9d-107">指派許可權給其信箱。</span><span class="sxs-lookup"><span data-stu-id="99e9d-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="99e9d-108">在 SharePoint 檔案共用中共用或刪除大量檔案。</span><span class="sxs-lookup"><span data-stu-id="99e9d-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="99e9d-109">建立 eDiscovery 搜尋並匯出搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="99e9d-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="99e9d-110">若要複查並對警示採取動作：</span><span class="sxs-lookup"><span data-stu-id="99e9d-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="99e9d-111">移至[安全性 & 合規性中心](https://protection.office.com)並登入。</span><span class="sxs-lookup"><span data-stu-id="99e9d-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="99e9d-112">按一下 [**提醒** > ] [**查看提醒**]。</span><span class="sxs-lookup"><span data-stu-id="99e9d-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="99e9d-113">按一下警示以顯示彈出頁面，包含提醒的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="99e9d-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="99e9d-114">您可以對警示採取動作，例如[移除可疑的收件匣規則](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)。</span><span class="sxs-lookup"><span data-stu-id="99e9d-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="99e9d-115">或者，您只要在 [警示飛出] 頁面上按一下 [**解析**]，即可關閉警示。</span><span class="sxs-lookup"><span data-stu-id="99e9d-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="99e9d-116">如需設定及管理報警原則的詳細資訊，請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="99e9d-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="99e9d-117">**重要**：警示來自 Microsoft 的電子郵件通知，永遠不會要求您執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="99e9d-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="99e9d-118">提供密碼</span><span class="sxs-lookup"><span data-stu-id="99e9d-118">Provide a password</span></span>
- <span data-ttu-id="99e9d-119">驗證帳戶的安全性詳細資料</span><span class="sxs-lookup"><span data-stu-id="99e9d-119">Verify the security details of your account</span></span>
- <span data-ttu-id="99e9d-120">重新驗證您的自我</span><span class="sxs-lookup"><span data-stu-id="99e9d-120">Re-authenticate yourself</span></span>

<span data-ttu-id="99e9d-121">如果您收到類似這封的電子郵件訊息，它並非 Microsoft 所傳送，應視為網路釣魚詐騙。</span><span class="sxs-lookup"><span data-stu-id="99e9d-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="99e9d-122">如果發生這種情況，請[向 Microsoft 報告](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。</span><span class="sxs-lookup"><span data-stu-id="99e9d-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>