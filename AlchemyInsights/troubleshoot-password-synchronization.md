---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279047"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="aba5d-102">疑難排解密碼同步處理</span><span class="sxs-lookup"><span data-stu-id="aba5d-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="aba5d-103">若要疑難排解其中沒有密碼會與 Azure AD 連接版本 1.1.614.0 同步處理或更新版本的問題：</span><span class="sxs-lookup"><span data-stu-id="aba5d-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="aba5d-104">開啟新的 Windows PowerShell 工作階段 Azure AD 連線伺服器上使用 [**以系統管理員身分執行**] 選項。</span><span class="sxs-lookup"><span data-stu-id="aba5d-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="aba5d-105">執行**Set-executionpolicy RemoteSigned**或**Set-executionpolicy Unrestricted**。</span><span class="sxs-lookup"><span data-stu-id="aba5d-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="aba5d-106">啟動 Azure AD 連線精靈]。</span><span class="sxs-lookup"><span data-stu-id="aba5d-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="aba5d-107">瀏覽至 [\* \* 其他工作 \* *] 頁面上，選取 [* \* Troubleshoot \* \*，然後按一下 [**下一步**。</span><span class="sxs-lookup"><span data-stu-id="aba5d-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="aba5d-108">疑難排解] 索引標籤上按一下 [**啟動疑難排解啟動**] 功能表中使用 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="aba5d-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="aba5d-109">在 [主要] 功能表中選取 [**疑難排解密碼同步處理**]。</span><span class="sxs-lookup"><span data-stu-id="aba5d-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="aba5d-110">子功能表中選取 [**密碼同步處理未完全運作**。</span><span class="sxs-lookup"><span data-stu-id="aba5d-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="aba5d-111">**了解疑難排解工作的結果**</span><span class="sxs-lookup"><span data-stu-id="aba5d-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="aba5d-112">疑難排解工作會執行下列檢查：</span><span class="sxs-lookup"><span data-stu-id="aba5d-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="aba5d-113">驗證的密碼同步處理功能已啟用 Azure AD 租用。</span><span class="sxs-lookup"><span data-stu-id="aba5d-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="aba5d-114">驗證 Azure AD 連線伺服器不是在執行模式。</span><span class="sxs-lookup"><span data-stu-id="aba5d-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="aba5d-115">每個現有內部部署 Active Directory 連接器 （這會對應至現有的 Active Directory 樹系）：</span><span class="sxs-lookup"><span data-stu-id="aba5d-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="aba5d-116">驗證已啟用密碼同步處理功能。</span><span class="sxs-lookup"><span data-stu-id="aba5d-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="aba5d-117">搜尋的 Windows 應用程式事件記錄檔中的密碼同步處理活動訊號事件。</span><span class="sxs-lookup"><span data-stu-id="aba5d-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="aba5d-118">每個 Active Directory 網域的內部部署 Active Directory 連接器底下：</span><span class="sxs-lookup"><span data-stu-id="aba5d-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="aba5d-119">驗證網域可從 Azure AD 連線伺服器。</span><span class="sxs-lookup"><span data-stu-id="aba5d-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="aba5d-120">驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務 (AD DS) 帳戶具有正確的使用者名稱、 密碼和密碼同步處理所需的權限。</span><span class="sxs-lookup"><span data-stu-id="aba5d-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="aba5d-121">密碼同步處理的疑難排解的詳細說明，請參閱 ＜ [Troubleshoot 密碼同步處理 Azure AD 連線同步處理](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="aba5d-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

