---
title: 處於擱置狀態的裝置
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652148"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="ecd23-102">處於擱置狀態的裝置</span><span class="sxs-lookup"><span data-stu-id="ecd23-102">Device in pending state</span></span>

<span data-ttu-id="ecd23-103">**先決條件：**</span><span class="sxs-lookup"><span data-stu-id="ecd23-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="ecd23-104">如果您是第一次設定裝置註冊，請確定您已在 [Azure Active Directory (AZURE ad) 中查看裝置管理的簡介 ](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) ，它會指導您如何在 azure ad 的控制下取得裝置。</span><span class="sxs-lookup"><span data-stu-id="ecd23-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="ecd23-105">如果您直接向 Azure AD 註冊裝置，並將其註冊到 Intune，您必須確定您已 [設定 intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) 並且先進行 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 。</span><span class="sxs-lookup"><span data-stu-id="ecd23-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="ecd23-106">確定您有權在 Azure AD 和內部部署 AD 中執行作業。</span><span class="sxs-lookup"><span data-stu-id="ecd23-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ecd23-107">只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。</span><span class="sxs-lookup"><span data-stu-id="ecd23-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ecd23-108">此外，如果您在內部部署 Active Directory 中設定自動註冊，您必須是 Active Directory 和 AD FS (的系統管理員（如果適用的話）) 。</span><span class="sxs-lookup"><span data-stu-id="ecd23-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ecd23-109">混合式 Azure AD join 註冊程式需要裝置在公司網路上。</span><span class="sxs-lookup"><span data-stu-id="ecd23-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="ecd23-110">它也會透過 VPN 運作，但有一些對該功能的忠告。</span><span class="sxs-lookup"><span data-stu-id="ecd23-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="ecd23-111">我們聽說客戶在遠端工作情況下，需要協助疑難排解混合式 Azure AD join 註冊程式。</span><span class="sxs-lookup"><span data-stu-id="ecd23-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="ecd23-112">**使用 Azure AD 密碼雜湊同步處理或透過驗證的雲端驗證環境 ()**</span><span class="sxs-lookup"><span data-stu-id="ecd23-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="ecd23-113">此註冊流程也稱為「同步加入」。</span><span class="sxs-lookup"><span data-stu-id="ecd23-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="ecd23-114">以下是註冊程式期間所發生狀況的分解：</span><span class="sxs-lookup"><span data-stu-id="ecd23-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="ecd23-115">Windows 10 探索服務連線點 (SCP 在使用者登入裝置時) 記錄。</span><span class="sxs-lookup"><span data-stu-id="ecd23-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="ecd23-116">裝置會先嘗試從登錄中的用戶端 SCP 中取得租使用者資訊 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。</span><span class="sxs-lookup"><span data-stu-id="ecd23-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="ecd23-117">如需詳細資訊，請參閱 [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。</span><span class="sxs-lookup"><span data-stu-id="ecd23-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="ecd23-118">如果失敗，裝置會與內部部署的 Active Directory 通訊，以取得來自 SCP 的承租人資訊。</span><span class="sxs-lookup"><span data-stu-id="ecd23-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="ecd23-119">若要驗證 SCP，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。</span><span class="sxs-lookup"><span data-stu-id="ecd23-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="ecd23-120">我們建議您在 Active Directory 中啟用 SCP，而且只能使用用戶端 SCP 進行初始驗證。</span><span class="sxs-lookup"><span data-stu-id="ecd23-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="ecd23-121">Windows 10 會嘗試與系統內容底下的 Azure AD 通訊，以針對 Azure AD 進行自我驗證。</span><span class="sxs-lookup"><span data-stu-id="ecd23-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="ecd23-122">您可以使用 [Test Device Registration Connectivity 腳本](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)，確認裝置是否可以存取系統帳戶底下的 Microsoft 資源。</span><span class="sxs-lookup"><span data-stu-id="ecd23-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="ecd23-123">Windows 10 會產生自我簽署憑證，並將其儲存在內部部署 Active Directory 中的 computer 物件底下。</span><span class="sxs-lookup"><span data-stu-id="ecd23-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="ecd23-124">這需要在網域控制站上進行直線。</span><span class="sxs-lookup"><span data-stu-id="ecd23-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="ecd23-125">具有憑證的裝置物件會透過 Azure AD Connect 同步處理至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="ecd23-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="ecd23-126">同步處理週期預設為每30分鐘，但是取決於 Azure AD Connect 的設定。</span><span class="sxs-lookup"><span data-stu-id="ecd23-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="ecd23-127">如需詳細資訊，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。</span><span class="sxs-lookup"><span data-stu-id="ecd23-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="ecd23-128">在此階段，您應該可以在 Azure 入口網站的裝置 blade 下，于「**擱置**」狀態看到主體裝置。</span><span class="sxs-lookup"><span data-stu-id="ecd23-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="ecd23-129">在下一個使用者登入至 Windows 10 時，註冊將會完成。</span><span class="sxs-lookup"><span data-stu-id="ecd23-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ecd23-130">如果您是在 VPN 上，且登出/登入已中斷網域連線，您可以手動觸發註冊。</span><span class="sxs-lookup"><span data-stu-id="ecd23-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="ecd23-131">若要執行這項作業，請完成下列程序：</span><span class="sxs-lookup"><span data-stu-id="ecd23-131">To do that:</span></span>
    >
    > <span data-ttu-id="ecd23-132">`dsregcmd /join`在本機上以系統管理員的身分，或透過 PSExec 從 PSExec 向您的電腦發佈。</span><span class="sxs-lookup"><span data-stu-id="ecd23-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="ecd23-133">例如：`PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="ecd23-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="ecd23-134">如需 Azure Active Directory 裝置註冊的常見問題，請參閱 [裝置常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq)。</span><span class="sxs-lookup"><span data-stu-id="ecd23-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
