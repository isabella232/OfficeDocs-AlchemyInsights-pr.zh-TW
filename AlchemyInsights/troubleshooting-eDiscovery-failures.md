---
title: 1490-疑難排解-eDiscovery-失敗
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277815"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="229bf-102">疑難排解內容搜尋錯誤</span><span class="sxs-lookup"><span data-stu-id="229bf-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="229bf-103">當您匯出搜尋結果時，是否遇到內容搜尋問題或取得失敗的問題？</span><span class="sxs-lookup"><span data-stu-id="229bf-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="229bf-104">例如，當您執行搜尋時，是否要接收下列專案？</span><span class="sxs-lookup"><span data-stu-id="229bf-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="229bf-105">CS008 或 CS012 錯誤</span><span class="sxs-lookup"><span data-stu-id="229bf-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="229bf-106">伺服器忙碌/逾時錯誤</span><span class="sxs-lookup"><span data-stu-id="229bf-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="229bf-107">發生應用程式錯誤</span><span class="sxs-lookup"><span data-stu-id="229bf-107">Application error occurred</span></span>

<span data-ttu-id="229bf-108">或是從大量信箱 100000 (的結果搜尋或匯出) 時，是否有您取得匯出的錯誤？</span><span class="sxs-lookup"><span data-stu-id="229bf-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="229bf-109">針對這些類型的錯誤，請嘗試對失敗的內容位置進行搜尋。</span><span class="sxs-lookup"><span data-stu-id="229bf-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="229bf-110">如需詳細資訊，請參閱  [本文](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 。</span><span class="sxs-lookup"><span data-stu-id="229bf-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="229bf-111">若要匯出的信箱超過10個，您必須使用下列 Powershell 下載匯出結果：  [從超過100k 的信箱匯出結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="229bf-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
