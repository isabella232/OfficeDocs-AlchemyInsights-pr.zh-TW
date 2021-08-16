---
title: Teams 系統管理中心
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049335"
---
# <a name="teams-admin-center"></a>Teams 系統管理中心

了解如何使用 [Teams 系統管理中心](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center) 來管理 Teams。

如果無法存取 Teams 系統管理中心，請檢查下列項目：

- 請確認您已在任何周邊裝置 (防火牆等)，或本機電腦上的防火牆規則中，允許適當的 [Office 365 IP 位址和 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)。
- 確認您用來存取 Teams 系統管理入口網站的登入與在 [Microsoft 365 系統管理入口網站](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)中所列的使用者名稱相符。

如果使用者未出現於 Teams 系統管理中心，請檢查下列項目：

- 您是否已在最近 24 小時內建立使用者或指派授權？ 請確定在開啟支援票證前，先等候至少 24 小時。
- 確認您已指派適當的授權？
- 如果您擁有內部部署的 Active Directory，請確認 [您的本機 Active Directory 中的 ProxyAddresses 欄位中的 msRTCSIP-PrimaryUserAddress 或 SIP 位址的值是唯一值，且格式符合](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip：[Microsoft 365 系統管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)的使用者的 **使用者名稱**。
- 如果您想要保留商務用 Skype Server 部署並讓使用者駐留于內部部署和線上：請參閱商務用 Skype Server [控制台] 中的 **[使用 Teams 和商務用 Skype Online 設定混合式部屬]** 並在線上移動使用者。
