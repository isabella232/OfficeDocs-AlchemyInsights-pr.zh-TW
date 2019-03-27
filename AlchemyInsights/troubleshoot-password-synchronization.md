---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767167"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="df352-102">疑難排解密碼同步處理</span><span class="sxs-lookup"><span data-stu-id="df352-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="df352-103">若要疑難排解其中沒有密碼會同步處理與 Azure AD Connect 版本 1.1.614.0 或更新版本的問題：</span><span class="sxs-lookup"><span data-stu-id="df352-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="df352-104">開啟新的 Windows PowerShell 工作階段，您的 Azure AD Connect 伺服器上具有 [**以管理員身分執行**] 選項。</span><span class="sxs-lookup"><span data-stu-id="df352-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="df352-105">執行**Set-executionpolicy RemoteSigned**或**Set-executionpolicy Unrestricted**。</span><span class="sxs-lookup"><span data-stu-id="df352-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="df352-106">啟動 Azure AD Connect 精靈。</span><span class="sxs-lookup"><span data-stu-id="df352-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="df352-107">瀏覽至 [\* \* 其他工作 \* *] 頁面上，選取 [* \* 疑難排解 \* \*，按一下 [**下一步**。</span><span class="sxs-lookup"><span data-stu-id="df352-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="df352-108">在 [疑難排解] 頁面上，按一下**要啟動的疑難排解啟動**] 功能表 PowerShell 中。</span><span class="sxs-lookup"><span data-stu-id="df352-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="df352-109">在 [主要] 功能表中，選取**疑難排解密碼同步處理**。</span><span class="sxs-lookup"><span data-stu-id="df352-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="df352-110">子功能表中，選取 [**密碼同步處理未完全運作**。</span><span class="sxs-lookup"><span data-stu-id="df352-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="df352-111">**了解疑難排解工作的結果**</span><span class="sxs-lookup"><span data-stu-id="df352-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="df352-112">疑難排解工作會執行下列檢查：</span><span class="sxs-lookup"><span data-stu-id="df352-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="df352-113">驗證您的 Azure AD 租用戶，已啟用密碼同步處理功能。</span><span class="sxs-lookup"><span data-stu-id="df352-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="df352-114">驗證 Azure AD Connect 伺服器不在執行模式。</span><span class="sxs-lookup"><span data-stu-id="df352-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="df352-115">每個現有內部部署 Active Directory 連接器 （這會對應至現有的 Active Directory 樹系）：</span><span class="sxs-lookup"><span data-stu-id="df352-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="df352-116">驗證已啟用密碼同步處理功能。</span><span class="sxs-lookup"><span data-stu-id="df352-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="df352-117">在 Windows 應用程式事件記錄檔的密碼同步處理活動訊號事件的搜尋。</span><span class="sxs-lookup"><span data-stu-id="df352-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="df352-118">每個 Active Directory 網域下的內部部署 Active Directory 連接器：</span><span class="sxs-lookup"><span data-stu-id="df352-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="df352-119">驗證的網域是可從 Azure AD Connect 伺服器。</span><span class="sxs-lookup"><span data-stu-id="df352-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="df352-120">驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務 (AD DS) 帳戶具有正確的使用者名稱、 密碼及權限所需的密碼同步處理。</span><span class="sxs-lookup"><span data-stu-id="df352-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="df352-121">疑難排解密碼同步處理的詳細說明，請參閱[使用 Azure AD Connect 同步處理的疑難排解密碼同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="df352-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

