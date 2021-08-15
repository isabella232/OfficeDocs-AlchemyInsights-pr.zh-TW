---
title: 由於錯誤 autologon.microsoftazuread-sso.com:443，無法登入 Teams
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038391"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>由於錯誤 autologon.microsoftazuread-sso.com:443，無法登入 Teams

如果將無縫 SSO 啟用為 O365 驗證，則可能需要將 URL “autologon.microsoftazuread-sso.com” 新增至內部網路網站。  如果已將它新增到信任的網站，且正在使用無縫 SSO，應將它從信任的網站中移除。

請參閱[無縫 SSO 疑難排解檢查清單](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)。

請按照下列步驟，將 URL 新增至內部網路網站清單：

1. 按一下 [開始] 按鈕來開啟 Internet Explorer。 在 [搜尋] 方塊中，輸入 [Internet Explorer]，然後在結果清單中按一下 [Internet Explorer]。
2. 按一下 [工具]，然後按一下 [網際網路選項]。
3. 按一下 [安全性] 索引標籤。
4. 現在，按一下 [本機內部網路網站] 然後按一下 [網站] 按鈕，然後按 [進階] 按鈕。
5. 輸入網站 URL，然後按一下 [新增]。
6. 完成後，按一下 [關閉]。

如需詳細資訊，請參閱[在 O365 中部署無縫 SSO 的文件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (包含原則式程序，以在步驟 3 中將 URL 新增至內部網路網站)。
