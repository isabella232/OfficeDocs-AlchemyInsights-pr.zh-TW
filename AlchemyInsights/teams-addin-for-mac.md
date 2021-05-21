---
title: Mac 版 Teams 增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582061"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="b8d44-102">Mac 版 Teams 增益集</span><span class="sxs-lookup"><span data-stu-id="b8d44-102">Teams add-in for Mac</span></span>

<span data-ttu-id="b8d44-103">若要為 Mac 作業系統使用者疑難排解遺漏 Teams 增益集的問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="b8d44-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="b8d44-104">**步驟 1：** 如果您使用混合式 Exchange 內部部署 (需要 2016 CU3 或更新版本)，請使用 Test-HMA.ps1 工具來確認已正確設定混合式新式驗證。</span><span class="sxs-lookup"><span data-stu-id="b8d44-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="b8d44-105">如需詳細資訊，請參閱[針對 iOS 和 Android 版 Outlook 驗證混合式新式驗證設定](https://aka.ms/TestHMAEAS)。</span><span class="sxs-lookup"><span data-stu-id="b8d44-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="b8d44-106">**注意：** 使用 UPN 位址格式 (例如，[username@contoso.com](mailto:username@contoso.com))，而非domain\username。</span><span class="sxs-lookup"><span data-stu-id="b8d44-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="b8d44-107">執行此動作，即使是對擁有 Exchange Online 信箱的使用者也這麼做。</span><span class="sxs-lookup"><span data-stu-id="b8d44-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="b8d44-108">**步驟 2：** 讓使用者在 Mac 版 Outlook 中移至 [工具 **]**  >  [帳戶 **]**，然後尋找並選取帳戶。</span><span class="sxs-lookup"><span data-stu-id="b8d44-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="b8d44-109">確認列出的使用者名稱為 UPN 格式 (例如，[username@contoso.com](mailto:username@contoso.com))。</span><span class="sxs-lookup"><span data-stu-id="b8d44-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="b8d44-110">**步驟 3：** 確認使用者為取得授權的 Microsoft Teams 使用者。</span><span class="sxs-lookup"><span data-stu-id="b8d44-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="b8d44-111">使用者必須使用 Mac 版 Office 365 訂閱，產品版本 16.24 或更新版本。</span><span class="sxs-lookup"><span data-stu-id="b8d44-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>