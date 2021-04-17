---
title: 疑難排解來自電子郵件的事件
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834830"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="9111c-102">疑難排解來自電子郵件的事件</span><span class="sxs-lookup"><span data-stu-id="9111c-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="9111c-103">確認已為信箱啟用該功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="9111c-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="9111c-104">然後查看「來自電子郵件的事件」記錄 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="9111c-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="9111c-105">在「來自電子郵件的事件」記錄中，找出與信箱中的項目相符的 InternetMessageId。</span><span class="sxs-lookup"><span data-stu-id="9111c-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="9111c-106">TrustScore 會決定是否要新增該項目。</span><span class="sxs-lookup"><span data-stu-id="9111c-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="9111c-107">只有當 TrustScore = "Trusted" 時，才會新增事件。</span><span class="sxs-lookup"><span data-stu-id="9111c-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="9111c-108">TrustScore 是由位於郵件標頭中的 SPF、Dkim 或 Dmarc 內容所決定。</span><span class="sxs-lookup"><span data-stu-id="9111c-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="9111c-109">若要檢視這些內容：</span><span class="sxs-lookup"><span data-stu-id="9111c-109">To view these properties:</span></span>

<span data-ttu-id="9111c-110">**電腦版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="9111c-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="9111c-111">開啟項目</span><span class="sxs-lookup"><span data-stu-id="9111c-111">Open the item</span></span>
- <span data-ttu-id="9111c-112">檔案 -> 內容 -> 網際網路標頭</span><span class="sxs-lookup"><span data-stu-id="9111c-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="9111c-113">或</span><span class="sxs-lookup"><span data-stu-id="9111c-113">or</span></span>

<span data-ttu-id="9111c-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="9111c-114">**MFCMapi**</span></span>

- <span data-ttu-id="9111c-115">導覽至收件匣中的項目</span><span class="sxs-lookup"><span data-stu-id="9111c-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="9111c-116">尋找 PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="9111c-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="9111c-117">這些內容會在傳輸和路由期間決定並記錄。</span><span class="sxs-lookup"><span data-stu-id="9111c-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="9111c-118">如需進一步的疑難排解，您可能需要追蹤關於 SPF、DKIM 和 DMARC 中失敗的傳輸支援。</span><span class="sxs-lookup"><span data-stu-id="9111c-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>