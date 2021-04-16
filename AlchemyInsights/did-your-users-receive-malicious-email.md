---
title: 您的使用者是否收到惡意電子郵件
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815237"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="6359f-102">您的使用者是否收到惡意電子郵件?</span><span class="sxs-lookup"><span data-stu-id="6359f-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="6359f-103">您現在可以使用[安全性與合規性中的 [管理員提交]](https://sip.protection.office.com/reportsubmission)，將惡意電子郵件報告給 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="6359f-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="6359f-104">系統會掃描 [管理員提交](https://sip.protection.office.com/reportsubmission)中所提交的郵件，然後下列結果將顯示在 **詳細資料** 飛出視窗頁面中：</span><span class="sxs-lookup"><span data-stu-id="6359f-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="6359f-105">寄件者在傳遞電子郵件時，電子郵件驗證是否失敗。</span><span class="sxs-lookup"><span data-stu-id="6359f-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="6359f-106">任何有關可能會影響或覆寫郵件決策的原則點擊的資訊。</span><span class="sxs-lookup"><span data-stu-id="6359f-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="6359f-107">目前的引爆結果，查看郵件中所含的 URL 或檔案是否惡意。</span><span class="sxs-lookup"><span data-stu-id="6359f-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="6359f-108">來自評級員 的意見反應</span><span class="sxs-lookup"><span data-stu-id="6359f-108">Feedback from graders</span></span>

<span data-ttu-id="6359f-109">如果發現覆寫，則應該會在幾分鐘內完成重新掃描。</span><span class="sxs-lookup"><span data-stu-id="6359f-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="6359f-110">如果電子郵件驗證中沒有任何問題，或傳遞不受覆寫影響，則評級員的意見反應可能需要多達一天的時間。</span><span class="sxs-lookup"><span data-stu-id="6359f-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="6359f-111">如果您不同意郵件、URL 或檔案上的最終決策 (封鎖與未封鎖)，請在一天后重新提交該郵件。</span><span class="sxs-lookup"><span data-stu-id="6359f-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="6359f-112">當您再次提交郵件後，決策變更的可能性相當高。</span><span class="sxs-lookup"><span data-stu-id="6359f-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="6359f-113">同時，您可以依照[本文](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)中的指示，從使用者的收件匣中移除惡意電子郵件。</span><span class="sxs-lookup"><span data-stu-id="6359f-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="6359f-114">擁有 Microsoft Defender for Office 365 的客戶可以：</span><span class="sxs-lookup"><span data-stu-id="6359f-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="6359f-115">使用[威脅總管 [尋找] 並 [刪除可疑的電子郵件]](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="6359f-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="6359f-116">[使用安全連結封鎖存取](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)惡意 URL</span><span class="sxs-lookup"><span data-stu-id="6359f-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="6359f-117">追蹤已點擊和已存取惡意 URL 的使用者：[查看網路釣魚 URL，然後點擊決策資料](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="6359f-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="6359f-118">手動[開始 [自動化調查]](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="6359f-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="6359f-119">請按照[防範惡意 URL 和檔案](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)中的指示來保護自己免受惡意檔案和 URL 的攻擊。</span><span class="sxs-lookup"><span data-stu-id="6359f-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>