---
title: 錯誤：此電腦上的規則不符合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782943"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="4dc8a-102">錯誤：此電腦上的規則不符合</span><span class="sxs-lookup"><span data-stu-id="4dc8a-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="4dc8a-103">若要查看此已知問題的更新狀態，請參閱[此電腦上的規則與 Microsoft Exchange 上](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)的規則不符</span><span class="sxs-lookup"><span data-stu-id="4dc8a-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="4dc8a-104">Outlook 小組已在組建12928.10000 中實施修正。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="4dc8a-105">此修正已在內幕人士內快速，並會在2020年6月晚移至每月通道。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="4dc8a-106">當您有固定的組建之後，您可能會看到 [您想要保留哪個規則？] 最後一次的提示。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="4dc8a-107">出現提示時選擇 [伺服器]，然後傳回 Outlook，然後重新啟用已停用的任何規則。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="4dc8a-108">在提供修正程式之前，請使用下列解決方法：</span><span class="sxs-lookup"><span data-stu-id="4dc8a-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="4dc8a-109">**解決方法**：在最近的報告中，發生在 Outlook desktop 中僅已建立用戶端規則的問題。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="4dc8a-110">若繼續遇到問題，請考慮刪除規則，然後在 OWA (Outlook Web App) 中只建立和編輯規則，直到問題解決為止。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="4dc8a-111">如果您無法手動刪除規則，您可以在啟動 Outlook 時執行 Outlook.exe/cleanrules.，以執行 Outlook 命令。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="4dc8a-112">這會刪除用戶端和伺服器規則。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="4dc8a-113">它會刪除 Outlook 設定檔中所有帳戶的所有規則。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="4dc8a-114">此命令會在命令列參數文章中進一步記載。</span><span class="sxs-lookup"><span data-stu-id="4dc8a-114">This command is further documented in the Command-line switches article.</span></span>

