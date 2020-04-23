---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732501"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e6770-102">疑難排解密碼同步處理</span><span class="sxs-lookup"><span data-stu-id="e6770-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e6770-103">若要疑難排解未與 Azure AD Connect 版本1.1.614.0 或更新版本同步處理的問題：</span><span class="sxs-lookup"><span data-stu-id="e6770-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="e6770-104">在 Azure AD Connect server 上使用 [以**系統管理員身分執行**] 選項開啟新的 Windows PowerShell 會話。</span><span class="sxs-lookup"><span data-stu-id="e6770-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e6770-105">執行**Set-ExecutionPolicy RemoteSigned**或**Set-ExecutionPolicy**不限限制。</span><span class="sxs-lookup"><span data-stu-id="e6770-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="e6770-106">啟動 Azure AD Connect 嚮導。</span><span class="sxs-lookup"><span data-stu-id="e6770-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e6770-107">流覽至 [**其他**工作] 頁面，選取 [**疑難排解**]，然後按 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="e6770-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="e6770-108">在 [疑難排解] 頁面上，按一下 [啟動]，**以啟動 PowerShell 中的疑難排解**功能表。</span><span class="sxs-lookup"><span data-stu-id="e6770-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="e6770-109">在主功能表中，選取 [**密碼同步處理疑難排解**]。</span><span class="sxs-lookup"><span data-stu-id="e6770-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="e6770-110">在 [子功能表] 中，選取 [**密碼同步處理] 根本無法運作**。</span><span class="sxs-lookup"><span data-stu-id="e6770-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="e6770-111">**瞭解疑難排解任務的結果**</span><span class="sxs-lookup"><span data-stu-id="e6770-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="e6770-112">疑難排解任務會執行下列檢查：</span><span class="sxs-lookup"><span data-stu-id="e6770-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="e6770-113">驗證您的 Azure AD 租使用者已啟用密碼同步處理功能。</span><span class="sxs-lookup"><span data-stu-id="e6770-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="e6770-114">驗證 Azure AD Connect 伺服器不在分段模式。</span><span class="sxs-lookup"><span data-stu-id="e6770-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="e6770-115">針對每個現有的內部部署 Active Directory 連接器（會對應至現有的 Active Directory 樹系）：</span><span class="sxs-lookup"><span data-stu-id="e6770-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="e6770-116">驗證 [密碼同步處理] 功能已啟用。</span><span class="sxs-lookup"><span data-stu-id="e6770-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="e6770-117">在 Windows 應用程式事件記錄檔中搜尋密碼同步處理心跳事件。</span><span class="sxs-lookup"><span data-stu-id="e6770-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="e6770-118">針對內部部署 Active Directory 連接器底下的每個 Active Directory 網域：</span><span class="sxs-lookup"><span data-stu-id="e6770-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="e6770-119">驗證是否可以從 Azure AD Connect 伺服器訪問網域。</span><span class="sxs-lookup"><span data-stu-id="e6770-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="e6770-120">驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務（AD DS）帳戶是否具有密碼同步處理所需的正確使用者名稱、密碼和許可權。</span><span class="sxs-lookup"><span data-stu-id="e6770-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="e6770-121">如需疑難排解密碼同步處理的詳細資訊，請參閱[使用 AZURE AD Connect Sync 疑難排解密碼同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。</span><span class="sxs-lookup"><span data-stu-id="e6770-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  