---
title: 疑難排解來自電子郵件的事件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44515971"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="188f9-102">疑難排解來自電子郵件的事件</span><span class="sxs-lookup"><span data-stu-id="188f9-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="188f9-103">確認已為信箱啟用該功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="188f9-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="188f9-104">然後查看「來自電子郵件的事件」記錄 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="188f9-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="188f9-105">在「來自電子郵件的事件」記錄中，找出與信箱中的項目相符的 InternetMessageId。</span><span class="sxs-lookup"><span data-stu-id="188f9-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="188f9-106">TrustScore 會決定是否要新增該項目。</span><span class="sxs-lookup"><span data-stu-id="188f9-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="188f9-107">只有當 TrustScore = "Trusted" 時，才會新增事件。</span><span class="sxs-lookup"><span data-stu-id="188f9-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="188f9-108">TrustScore 是由位於郵件標頭中的 SPF、Dkim 或 Dmarc 內容所決定。</span><span class="sxs-lookup"><span data-stu-id="188f9-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="188f9-109">若要檢視這些內容：</span><span class="sxs-lookup"><span data-stu-id="188f9-109">To view these properties:</span></span>

<span data-ttu-id="188f9-110">**電腦版 Outlook**</span><span class="sxs-lookup"><span data-stu-id="188f9-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="188f9-111">開啟項目</span><span class="sxs-lookup"><span data-stu-id="188f9-111">Open the item</span></span>
- <span data-ttu-id="188f9-112">檔案 -> 內容 -> 網際網路標頭</span><span class="sxs-lookup"><span data-stu-id="188f9-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="188f9-113">或</span><span class="sxs-lookup"><span data-stu-id="188f9-113">or</span></span>

<span data-ttu-id="188f9-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="188f9-114">**MFCMapi**</span></span>

- <span data-ttu-id="188f9-115">導覽至收件匣中的項目</span><span class="sxs-lookup"><span data-stu-id="188f9-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="188f9-116">尋找 PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="188f9-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="188f9-117">這些內容會在傳輸和路由期間決定並記錄。</span><span class="sxs-lookup"><span data-stu-id="188f9-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="188f9-118">如需進一步的疑難排解，您可能需要追蹤關於 SPF、DKIM 和 DMARC 中失敗的傳輸支援。</span><span class="sxs-lookup"><span data-stu-id="188f9-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>