---
title: 支援的訂閱類型
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072151"
---
# <a name="supported-subscription-types"></a>支援的訂閱類型

請查看支援的訂閱類型以繼續進行。

[支援的訂閱類型](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**轉移帳單擁有權**

[Microsoft Azure 入口網站] 為計費帳戶的 [帳戶系統管理員](https://ms.portal.azure.com/)，該帳戶含有您想要轉移的訂閱

- 在 **成本管理 + 計費** 上搜尋。 從左方窗格中選取 **訂閱**。 依據存取權而定，您可能需要選取計費範圍，然後 **訂閱** 或 **Azure 訂閱**。
- 針對您想要轉移的訂閱，選取 [轉移帳單擁有權]
- 輸入使用者的電子郵件地址，其為訂閱的新擁有者帳戶的計費管理員，然後選取 **傳送轉移要求**
- 使用者會收到一封電子郵件，其中包含檢閱您的轉移要求的指示。 若要核准轉移要求，使用者會選取電子郵件中的連結，並遵循指示操作。

注意事項：如果您將您的訂閱帳單擁有權轉移至另一個 Azure AD 租用戶的使用者帳戶，在訂閱中用以管理資源的所有 [角色型存取控制 (RBAC) ](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)作業皆會永久移除。 只有新擁有者才有權管理訂閱中的資源。 如需詳細資訊，請參閱 [將訂閱轉移到另一個 Azure AD 租用戶中的使用者](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。

**轉移訂閱的擁有權**

[訂閱擁有者轉移] 必須有角色型存取控制(RBAC) 以管理訂閱中的資源失去其存取權。 如需有關將現有的訂閱新增至租用戶的詳細資訊，請參閱 [關聯或新增一個 Azure 訂閱至 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。

- 在目前計費週期中有現有未付金額的 [訂閱轉移] ，將不會轉移到新帳戶的新付款方式。 新帳戶使用者唯一能使用的資訊只有上個月的訂閱費用。 其餘的使用和計費記錄都不會隨訂閱轉移。
- Enterprise 合約 (EA) 訂閱的 [轉移帳單擁有權] 目前僅在 Enterprise 合約入口網站中支援。
- 將信用卡級訂閱 (例如 Visual Studio、BizSpark、Microsoft 合作夥伴網路) 轉移到新的使用者，需要有 Visual Studio/Microsoft 合作夥伴網路授權才能接受轉移要求
- 所有的資源像是虛擬機器、磁碟和網站成功地轉移到新帳戶。 在跨租用戶的訂閱轉移中，下列資源可能會受到影響：

**Azure AD Domain Services**

Azure Key Vaults

- [SQL 相關使用者和資料庫](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) 可能會受到影響，特別是如果客戶使用 Azure Active Directory 相關的驗證
- 使用 Azure Active Directory 驗證設定的 **應用程式服務** 可能會受到影響
- 當已連結的 Azure 訂閱取消時，已連線到 Azure 訂閱的 **Visual Studio Team** 服務帳戶可能會暫時無法存取。

**建議的文件**

接受帳單擁有權之後的步驟：

- 若要保留帳單擁有權，但變更您的訂閱類型，請參照：[將您的 Azure 訂閱切換到其他方案](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [傳送 Visual Studio、Microsoft 合作夥伴網路 (MPN) 和 [預付方案] 開發/測試訂閱](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [[企業合約 (EA)] 訂閱的轉移帳單擁有權](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [轉移擁有權常見問題](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [轉移擁有權問題的疑難排解](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)