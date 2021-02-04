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
# <a name="enable-password-writeback-in-azure-ad-connect"></a>在 Azure AD Connect 中啟用密碼回寫

若要啟用自助密碼重設回寫，請先在 Azure AD Connect 中啟用回寫選項。 從您的 Azure AD Connect 伺服器，完成下列步驟：

1. 登入您的 Azure AD Connect 伺服器，並啟動 **Azure AD Connect** 設定精靈。
2. 在 **[歡迎]** 頁面上，按一下 **[設定]**。
3. 在 **[其他工作]** 頁面上，選取 **[自訂同步處理選項]**，然後按 **[下一步]**。
4. 在 **[連線至 Azure AD]** 頁面上，輸入您 Azure 租用戶的全域系統管理員認證，然後按 **[下一步]**。
5. 在 **[連線目錄]** 和 **[網域/OU]** 篩選頁面上，按 **[下一步]**。
6. 在 **[選擇性功能]** 頁面上，選取 **[密碼回寫]** 旁的方塊，並按 **[下一步]**。
7. 在 **[已可設定]** 頁面上，按一下 **[設定]** 並等待程序完成。
8. 當您看到設定完成時，請按一下 **[結束]**。

在 Azure AD Connect 中啟用密碼回寫之後，設定 Azure AD SSPR 進行回寫。  若要在 SSPR 中啟用密碼回寫，請完成下列步驟：

1. 使用全域系統管理員帳戶登入 Azure 入口網站。
2. 搜尋並選取 **[Azure Active Directory]**，按一下 **[密碼重設]**，然後按一下 **[內部部署整合]**。
3. 將 **[要將密碼寫回您的內部部署目錄嗎?]** 選項設定為 **[是]**。
4. 將 **[允許使用者僅將帳戶解除鎖定而不重設密碼嗎?]** 選項設定為 **[是]**。
5. 準備好時，按一下 **[儲存]**。

如需詳細資訊，請參閱[啟用 Azure Active Directory 自助密碼重設回寫至內部部署環境](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)。

> [!NOTE]
>  當管理員在 Azure 入口網站中重設使用者密碼時，如果該使用戶已同盟或同步密碼雜湊，則密碼將寫回內部部署。 此功能需要 Azure 進階授權 (P1 or P2)，且目前不在 Office 管理入口網站中支援。
