---
title: 疑難排解 PRT 問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571877"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="bca38-102">疑難排解 PRT 問題</span><span class="sxs-lookup"><span data-stu-id="bca38-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="bca38-103">若要讓任何裝置完成取得驗證，必須完全註冊且狀態良好，且能夠 (PRT) 取得主要重新整理權杖。</span><span class="sxs-lookup"><span data-stu-id="bca38-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="bca38-104">混合式 Azure AD join 註冊程式需要裝置在公司網路上。</span><span class="sxs-lookup"><span data-stu-id="bca38-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="bca38-105">它也會透過 VPN 運作，但有一些對該功能的忠告。</span><span class="sxs-lookup"><span data-stu-id="bca38-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="bca38-106">在遠端工作情況下，我們已聽說客戶需要協助疑難排解混合式 Azure AD join 註冊程式。</span><span class="sxs-lookup"><span data-stu-id="bca38-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="bca38-107">以下是在註冊過程中，出現在「蓋子」下的情況明細。</span><span class="sxs-lookup"><span data-stu-id="bca38-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="bca38-108">**使用 Azure AD 密碼雜湊同步處理或透過驗證的雲端驗證環境 ()**</span><span class="sxs-lookup"><span data-stu-id="bca38-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="bca38-109">此註冊流程也稱為「同步加入」。</span><span class="sxs-lookup"><span data-stu-id="bca38-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="bca38-110">Windows 10 會在使用者登入裝置時搜尋 SCP 記錄。</span><span class="sxs-lookup"><span data-stu-id="bca38-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="bca38-111">裝置會先嘗試從登錄中的用戶端 SCP 中取得租使用者資訊 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。</span><span class="sxs-lookup"><span data-stu-id="bca38-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="bca38-112">如需詳細資訊，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。</span><span class="sxs-lookup"><span data-stu-id="bca38-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="bca38-113">若失敗，裝置會與內部部署 Active Directory (AD) 進行通訊，以從服務連線點 (SCP) 取得租使用者資訊。</span><span class="sxs-lookup"><span data-stu-id="bca38-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="bca38-114">若要驗證 SCP，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。</span><span class="sxs-lookup"><span data-stu-id="bca38-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="bca38-115">我們建議您在 AD 中啟用 SCP，且只使用用戶端 SCP 進行初始驗證。</span><span class="sxs-lookup"><span data-stu-id="bca38-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="bca38-116">Windows 10 會嘗試與系統內容底下的 Azure AD 通訊，以針對 Azure AD 進行自我驗證。</span><span class="sxs-lookup"><span data-stu-id="bca38-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="bca38-117">您可以使用 Test Device Registration Connectivity 腳本，確認裝置是否可以存取系統帳戶底下的 Microsoft 資源。</span><span class="sxs-lookup"><span data-stu-id="bca38-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="bca38-118">Windows 10 會產生自我簽署憑證，並將它儲存在內部部署 AD 中的 computer 物件底下。</span><span class="sxs-lookup"><span data-stu-id="bca38-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="bca38-119">這需要在網域控制站上進行直線。</span><span class="sxs-lookup"><span data-stu-id="bca38-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="bca38-120">具有憑證的裝置物件會透過 Azure AD Connect 同步處理至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="bca38-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="bca38-121">同步處理週期預設為每30分鐘，但是取決於 Azure AD Connect 的設定。</span><span class="sxs-lookup"><span data-stu-id="bca38-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="bca38-122">如需詳細資訊，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。</span><span class="sxs-lookup"><span data-stu-id="bca38-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="bca38-123">在此階段，您應該可以在 Azure 入口網站的裝置 blade 下，于「擱置」狀態看到主體裝置。</span><span class="sxs-lookup"><span data-stu-id="bca38-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="bca38-124">在下一個使用者登入至 Windows 10 時，註冊將會完成。</span><span class="sxs-lookup"><span data-stu-id="bca38-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="bca38-125">如果您使用的是 VPN，且登出登入程式會終止網域連線，您可以手動觸發註冊：</span><span class="sxs-lookup"><span data-stu-id="bca38-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="bca38-126">在以系統管理提示或從 PSExec 遠端透過 PSExec 向您的電腦發出 dsregcmd/join。</span><span class="sxs-lookup"><span data-stu-id="bca38-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="bca38-127">例如，PsExec-s \\ win10client01 cmd，dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="bca38-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="bca38-128">如需混合式加入問題的詳細資訊，請參閱 [裝置問題疑難排解](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)。</span><span class="sxs-lookup"><span data-stu-id="bca38-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
