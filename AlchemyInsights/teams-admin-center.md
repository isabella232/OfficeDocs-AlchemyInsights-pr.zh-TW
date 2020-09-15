---
title: Teams 系統管理中心
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670355"
---
# <a name="teams-admin-center"></a><span data-ttu-id="f3086-102">Teams 系統管理中心</span><span class="sxs-lookup"><span data-stu-id="f3086-102">Teams Admin Center</span></span>

<span data-ttu-id="f3086-103">了解如何使用 [Teams 系統管理中心](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center) 來管理 Teams。</span><span class="sxs-lookup"><span data-stu-id="f3086-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="f3086-104">如果無法存取 Teams 系統管理中心，請檢查下列項目：</span><span class="sxs-lookup"><span data-stu-id="f3086-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="f3086-105">請確認您已在任何周邊裝置 (防火牆等)，或本機電腦上的防火牆規則中，允許適當的 [Office 365 IP 位址和 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)。</span><span class="sxs-lookup"><span data-stu-id="f3086-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="f3086-106">確認您用來存取 Teams 系統管理入口網站的登入與在 [Microsoft 365 系統管理入口網站](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中所列的使用者名稱相符。</span><span class="sxs-lookup"><span data-stu-id="f3086-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="f3086-107">如果使用者未出現於 Teams 系統管理中心，請檢查下列項目：</span><span class="sxs-lookup"><span data-stu-id="f3086-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="f3086-108">您是否已在最近 24 小時內建立使用者或指派授權？</span><span class="sxs-lookup"><span data-stu-id="f3086-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="f3086-109">請確定在開啟支援票證前，先等候至少 24 小時。</span><span class="sxs-lookup"><span data-stu-id="f3086-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="f3086-110">確認您已指派適當的授權？</span><span class="sxs-lookup"><span data-stu-id="f3086-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="f3086-111">如果您擁有內部部署的 Active Directory，請確認 [您的本機 Active Directory 中的 ProxyAddresses 欄位中的 msRTCSIP-PrimaryUserAddress 或 SIP 位址的值是唯一值，且格式符合 ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip：[Microsoft 365 系統管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)的使用者的**使用者名稱**。</span><span class="sxs-lookup"><span data-stu-id="f3086-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="f3086-112">如果您想要保留商務用 Skype Server 部署並讓使用者駐留于內部部署和線上：請參閱商務用 Skype Server [控制台] 中的 **[使用 Teams 和商務用 Skype Online 設定混合式部屬]** 並在線上移動使用者。</span><span class="sxs-lookup"><span data-stu-id="f3086-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
