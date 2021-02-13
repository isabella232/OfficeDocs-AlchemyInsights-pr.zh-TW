---
title: 密碼寫回無法運作
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232679"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="9db7b-102">密碼寫回無法運作</span><span class="sxs-lookup"><span data-stu-id="9db7b-102">Password Writeback is not working</span></span>

<span data-ttu-id="9db7b-103">**設定密碼寫回時有問題**</span><span class="sxs-lookup"><span data-stu-id="9db7b-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="9db7b-104">密碼寫回是一項高級功能。</span><span class="sxs-lookup"><span data-stu-id="9db7b-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="9db7b-105">請務必瞭解授權需求：</span><span class="sxs-lookup"><span data-stu-id="9db7b-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="9db7b-106">您的組織中必須至少有一個指派的授權</span><span class="sxs-lookup"><span data-stu-id="9db7b-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="9db7b-107">**僅限雲端使用者** -任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="9db7b-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="9db7b-108">**雲端和/或內部部署使用者** -Azure AD Premium P1 或 P2、Enterprise 可移動性 + SECURITY (EMS) 或安全生產力 (SPE) </span><span class="sxs-lookup"><span data-stu-id="9db7b-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="9db7b-109">若要深入瞭解授權需求，請參閱 [AZURE AD 自助密碼重設的授權需求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="9db7b-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="9db7b-110">您有至少一個系統管理員帳戶和一個具有適當授權的測試使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="9db7b-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="9db7b-111">您必須將 Azure AD Connect 連線至網域主控站模擬器，以供密碼寫回工作使用。</span><span class="sxs-lookup"><span data-stu-id="9db7b-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="9db7b-112">您可以設定 Azure AD Connect，以使用主要的網域控制站，方法是在 Active Directory 同步處理連接器的 **屬性** 上按一下滑鼠右鍵，然後選取 [ **設定目錄磁碟分割**]。</span><span class="sxs-lookup"><span data-stu-id="9db7b-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="9db7b-113">從那裡，尋找 [ **網域控制站連線設定** ] 區段，然後選取 [ **只使用偏好的網域控制站**] 方塊。</span><span class="sxs-lookup"><span data-stu-id="9db7b-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="9db7b-114">如果首選 DC 不是 PDC 模擬器，Azure AD Connect 仍會到達 PDC 以進行密碼回寫。</span><span class="sxs-lookup"><span data-stu-id="9db7b-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="9db7b-115">已在您的租使用者中設定並啟用密碼重設。</span><span class="sxs-lookup"><span data-stu-id="9db7b-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="9db7b-116">如需詳細資訊，請參閱 [讓使用者重設其 AZURE AD 密碼](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)。</span><span class="sxs-lookup"><span data-stu-id="9db7b-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="9db7b-117">確定要用來啟用密碼寫回的系統管理員帳戶， (Azure AD 中建立的雲端系統管理員帳戶不在內部部署 AD) </span><span class="sxs-lookup"><span data-stu-id="9db7b-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="9db7b-118">您有一個或多個樹系 AD 內部部署執行 Windows Server 2008 R2、Windows Server 2012 或 Windows Server 2012 R2 （安裝了最新的 service pack）</span><span class="sxs-lookup"><span data-stu-id="9db7b-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="9db7b-119">您已安裝 Azure AD Connect 工具，且已準備好要同步處理至雲端的 AD 環境。</span><span class="sxs-lookup"><span data-stu-id="9db7b-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="9db7b-120">在測試密碼寫回之前，請先確定您已完成從 Azure AD Connect 中的 AD 和 Azure AD 的完整匯入和完整同步處理。</span><span class="sxs-lookup"><span data-stu-id="9db7b-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="9db7b-121">若要深入瞭解，請參閱如何 [在 AZURE AD Connect 中執行完整同步和完整匯入](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="9db7b-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="9db7b-122">**我在密碼寫回連線時出現問題**</span><span class="sxs-lookup"><span data-stu-id="9db7b-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="9db7b-123">下載並啟用[AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)的最新版本</span><span class="sxs-lookup"><span data-stu-id="9db7b-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="9db7b-124">防火牆設定： Azure AD Connect 工具 (1.1.443 及更新版本) 需要 **輸出 HTTPS** 存取權：</span><span class="sxs-lookup"><span data-stu-id="9db7b-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="9db7b-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="9db7b-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="9db7b-126">windows 網路</span><span class="sxs-lookup"><span data-stu-id="9db7b-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="9db7b-127">允許閒置連線至少保留2-3 分鐘</span><span class="sxs-lookup"><span data-stu-id="9db7b-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="9db7b-128">**密碼回寫時仍然存在問題**</span><span class="sxs-lookup"><span data-stu-id="9db7b-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="9db7b-129">如果您仍然有困難，請嘗試停用並重新啟用 Azure AD Connect 工具中的密碼回寫服務。</span><span class="sxs-lookup"><span data-stu-id="9db7b-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="9db7b-130">若要深入瞭解，請參閱如何 [停用及重新啟用密碼回寫功能](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="9db7b-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
