---
title: 在 Azure AD Connect 中啟用密碼回寫
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093346"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="408ec-102">在 Azure AD Connect 中啟用密碼回寫</span><span class="sxs-lookup"><span data-stu-id="408ec-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="408ec-103">若要啟用自助密碼重設回寫，請先在 Azure AD Connect 中啟用回寫選項。</span><span class="sxs-lookup"><span data-stu-id="408ec-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="408ec-104">從您的 Azure AD Connect 伺服器，完成下列步驟：</span><span class="sxs-lookup"><span data-stu-id="408ec-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="408ec-105">登入您的 Azure AD Connect 伺服器，並啟動 **Azure AD Connect** 設定精靈。</span><span class="sxs-lookup"><span data-stu-id="408ec-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="408ec-106">在 **[歡迎]** 頁面上，按一下 **[設定]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="408ec-107">在 **[其他工作]** 頁面上，選取 **[自訂同步處理選項]**，然後按 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="408ec-108">在 **[連線至 Azure AD]** 頁面上，輸入您 Azure 租用戶的全域系統管理員認證，然後按 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="408ec-109">在 **[連線目錄]** 和 **[網域/OU]** 篩選頁面上，按 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="408ec-110">在 **[選擇性功能]** 頁面上，選取 **[密碼回寫]** 旁的方塊，並按 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="408ec-111">在 **[已可設定]** 頁面上，按一下 **[設定]** 並等待程序完成。</span><span class="sxs-lookup"><span data-stu-id="408ec-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="408ec-112">當您看到設定完成時，請按一下 **[結束]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="408ec-113">在 Azure AD Connect 中啟用密碼回寫之後，設定 Azure AD SSPR 進行回寫。</span><span class="sxs-lookup"><span data-stu-id="408ec-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="408ec-114">若要在 SSPR 中啟用密碼回寫，請完成下列步驟：</span><span class="sxs-lookup"><span data-stu-id="408ec-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="408ec-115">使用全域系統管理員帳戶登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="408ec-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="408ec-116">搜尋並選取 **[Azure Active Directory]**，按一下 **[密碼重設]**，然後按一下 **[內部部署整合]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="408ec-117">將 **[要將密碼寫回您的內部部署目錄嗎?]** 選項設定為 **[是]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="408ec-118">將 **[允許使用者僅將帳戶解除鎖定而不重設密碼嗎?]** 選項設定為 **[是]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="408ec-119">準備好時，按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="408ec-119">When ready, click **Save**.</span></span>

<span data-ttu-id="408ec-120">如需詳細資訊，請參閱[啟用 Azure Active Directory 自助密碼重設回寫至內部部署環境](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)。</span><span class="sxs-lookup"><span data-stu-id="408ec-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="408ec-121">當管理員在 Azure 入口網站中重設使用者密碼時，如果該使用戶已同盟或同步密碼雜湊，則密碼將寫回內部部署。</span><span class="sxs-lookup"><span data-stu-id="408ec-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="408ec-122">此功能需要 Azure 進階授權 (P1 or P2)，且目前不在 Office 管理入口網站中支援。</span><span class="sxs-lookup"><span data-stu-id="408ec-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
