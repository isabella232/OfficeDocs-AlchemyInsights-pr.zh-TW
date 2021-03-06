---
title: 設定供給服務
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480745"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="a60c3-102">設定供給服務</span><span class="sxs-lookup"><span data-stu-id="a60c3-102">Configuring the Provision service</span></span>

<span data-ttu-id="a60c3-103">為了讓自動化的使用者布建能夠運作，Azure AD 需要有效的認證，以允許其連線至 Workday Web 服務 API。</span><span class="sxs-lookup"><span data-stu-id="a60c3-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="a60c3-104">此外，在 Workday 至 AD 使用者布建應用程式上的 [測試連線] 按鈕，也會驗證是否可以連線至與 AD 網域相關聯的 Azure AD Connect 布布布建代理程式。</span><span class="sxs-lookup"><span data-stu-id="a60c3-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="a60c3-105">如果 Azure 入口網站在儲存認證時傳回錯誤，請遵循下列建議步驟：</span><span class="sxs-lookup"><span data-stu-id="a60c3-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="a60c3-106">請確認您已依照 [教學課程] 區段 [設定 workday 中的 Integration System 使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)所述，設定 Workday 整合系統使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="a60c3-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="a60c3-107">請確認 Azure AD Connect 布建代理程式服務已啟動，且已在內部部署 Windows server 上使用服務管理主控台執行。</span><span class="sxs-lookup"><span data-stu-id="a60c3-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="a60c3-108">您也可以在 Azure 入口網站中，按一下 [查看內部部署代理程式] 按鈕，檢查代理程式的狀態。</span><span class="sxs-lookup"><span data-stu-id="a60c3-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="a60c3-109">請務必使用 username@workday-租使用者名稱的格式，輸入 "Workday Username" 欄位的值。</span><span class="sxs-lookup"><span data-stu-id="a60c3-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="a60c3-110">如果 workday-租使用者名稱缺失，Workday 驗證會失敗。</span><span class="sxs-lookup"><span data-stu-id="a60c3-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="a60c3-111">若要設定與 Workday 實施租使用者的整合，請注意 Workday 租使用者的排程停機時間。</span><span class="sxs-lookup"><span data-stu-id="a60c3-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="a60c3-112">Workday 的實施租使用者排定停機時間的期限超過週末 (通常從星期五晚上到星期六早上) 和此停機時間的連線失敗] 視窗是一種已知的問題，可在實施承租人傳回線上時自動解決。</span><span class="sxs-lookup"><span data-stu-id="a60c3-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="a60c3-113">在極少的情況下，如果整合系統使用者的密碼因租使用者重新整理或帳戶處於鎖定或過期狀態，您也會看到此錯誤。</span><span class="sxs-lookup"><span data-stu-id="a60c3-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="a60c3-114">請使用 Workday 管理員檢查整合系統使用者的狀態。</span><span class="sxs-lookup"><span data-stu-id="a60c3-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="a60c3-115">如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="a60c3-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
