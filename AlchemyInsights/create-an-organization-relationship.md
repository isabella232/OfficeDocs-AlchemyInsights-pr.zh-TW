---
title: 建立組織關聯性以允許您的使用者與其他組織共同作業
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
- "3800014"
- "898"
ms.openlocfilehash: 5ea0f3dd2c1e21455b4750afbf9c43c931ad34bf357e94dd604ffe5bcdd2fa64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080341"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>建立組織關聯性以允許您的使用者與其他組織共同作業

1. 從 Microsoft 365 系統管理中心儀表板，移至 [系統管理]  >  [Exchange]。
2. 移至 [組織]  >  [共用]。
3. 在 [組織共用] 下，按一下 [新增]。
4. 在 [新增組織關聯性] 的 [關聯性名稱] 方塊中，為組織關聯性輸入易記名稱。
5. 在 **[網域共用對象]** 方塊中，輸入想要讓其查看您的行事曆的外部 Office 365 或 Exchange 內部部署組織的網域。如果您需要輸入多個網域，請使用逗號分隔網域名稱。例如， contoso.com, service.contoso.com。
6. 選取 [啟用行事曆空閒/忙碌資訊共用] 核取方塊，以開啟與您所列之網域的行事曆共用。設定行事曆空閒/忙碌資訊的共用層級，並設定哪些使用者可共用行事曆空閒/忙碌資訊。  

若要設定空閒/忙碌存取層級，請選擇下列其中一項：

- **只含時間的行事曆空閒/忙碌資訊**
- **行事曆空閒/忙碌的時間、主題與地點資訊**  

 若要設定將共用行事曆空閒/忙碌資訊的使用者，請選取下列其中一項：

- **組織中的所有人**
- **指定的安全性群組**  

按一下 [瀏覽] 以從清單中挑選安全性群組，然後按一下 [確定]。

按一下 [儲存] 來建立組織關聯性。  

**注意：** 跨租用戶設定不支援個人連絡人的空閒/忙碌查閱。 若要讓空閒/忙碌查閱可運作，必須將連絡人包含在全域通訊清單中。

**如需深入了解本主題，請參閱：**

- [在 Exchange Online 中建立組織關聯性](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [在 Exchange Online 中修改組織關聯性](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [在 Exchange Online 中移除組織關聯性](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
