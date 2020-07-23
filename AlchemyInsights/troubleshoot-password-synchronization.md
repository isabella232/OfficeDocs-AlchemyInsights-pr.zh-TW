---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387868"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="2b1ed-102">疑難排解密碼同步處理</span><span class="sxs-lookup"><span data-stu-id="2b1ed-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="2b1ed-103">若要疑難排解密碼同步處理問題，請從使用此 AAD Connect 疑難排解工作開始，以判斷密碼未同步處理的原因。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="2b1ed-104">若要開始，請移至「[管理直接同步](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)處理」。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="2b1ed-105">在 Azure AD Connect server 上開啟新的 Windows PowerShell 會話，然後選取 [以**系統管理員身分執行**] 選項。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="2b1ed-106">執行 Set-ExecutionPolicy RemoteSigned 或 Set-ExecutionPolicy 不限限制。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="2b1ed-107">啟動 Azure AD Connect 嚮導。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="2b1ed-108">移至 [其他工作] 頁面 >**疑難排解**  >  **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="2b1ed-109">選取 [**啟動**]，以開啟 [PowerShell 疑難排解] 功能表。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="2b1ed-110">選取 **[密碼同步處理疑難排解**]。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="2b1ed-111">此問題通常是不會同步處理特定使用者帳戶的密碼。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="2b1ed-112">**附注**如果最後一次成功的密碼同步處理是一段時間，則密碼同步處理會失敗。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="2b1ed-113">如需疑難排解密碼同步處理的詳細資訊，請參閱[使用 AZURE AD Connect Sync 疑難排解密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="2b1ed-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>