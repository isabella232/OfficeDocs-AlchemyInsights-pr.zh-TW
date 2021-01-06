---
title: 如何新增及管理系統管理員-建議的步驟
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755826"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>如何新增及管理系統管理員-建議的步驟

根據您的問題描述，我們找到您的解決方案。 當您遵循我們的檔後，大多數客戶都可以自行解決他們的問題。

**編輯訂閱管理員或共同管理員**

- 帳戶管理員可以編輯這兩個角色，而訂閱管理員只能在 [Azure 入口網站](https://ms.portal.azure.com/#home)中變更共同管理員。
- [新增或變更 Azure 訂閱管理員](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**更新內部 (的訂閱管理員或 Co-Administrator) 訂閱。**

服務管理員或共同系統管理員可以使用下列步驟，自行服務此動作：

1. 登入 [Azure 入口網站](https://ms.portal.azure.com/#home) ，然後按一下左刀片中的 [ **成本管理 + 帳單** ]。
2. 按一下行專案與您的訂閱。 這會開啟您訂閱的概述。
3. 在 **訂閱** blade 上，按一下 [ **屬性**]。 
4. 按一下 [ **服務管理員** ] 按鈕。
5. 輸入您要設定為服務管理員之使用者的電子郵件，然後按一下 **[確定]**。

**新增/變更/移除共同管理員**

1. 以服務管理員身分登入 [Azure 入口網站](https://ms.portal.azure.com/#home) 。
2. 開啟 [訂閱](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 並選取訂閱。  (共同管理員只能在訂閱範圍內指派。 ) 
3. 流覽至 **Access control (IAM)**  >  **傳統系統管理員**  >  **新增**  >  [**新增共同管理員**] 以開啟 [**新增** 共同管理員] 窗格。 (如果 [新增共同管理員] 選項已停用，則表示您沒有) 的許可權。
4. 選取您要新增的使用者，然後按一下 [ **新增**]。

**瞭解更多資訊：**
- [新增共同管理員](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [移除共同管理員](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [變更服務管理員](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [查看帳戶管理員](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [使用 RBAC 和 Azure 入口網站管理存取權](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**使用 Azure Active Directory (AD) 新增/刪除使用者**

您可以從 Azure Active Directory (Azure AD) 組織中新增或刪除現有的使用者：

1. 若要新增使用者，請以組織的使用者管理員身分登入 [Azure 入口網站](https://ms.portal.azure.com/#home) 。
2. 選取 [ **Azure Active Directory**]，選取 [ **使用者** ]，然後按一下 [ **新增使用者**]。
3. 在 [ **使用者** ] 頁面上，填寫必要的資訊。 按一下 [建立 **]**。 使用者建立並新增至您的 Azure AD 租使用者。

**深入瞭解**：

- [新增使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [刪除使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [使用 Azure Active Directory 新增或更新使用者的設定檔資訊](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**建議的檔**

- [什麼是以角色為基礎的存取控制 (RBAC) ？](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [瞭解 Azure 中的不同角色](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory 中的系統管理員角色權限](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [教學課程：授與使用 RBAC 和 Azure 入口網站的使用者存取](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [疑難排解 Azure 中的 RBAC](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [使用 Azure 管理群組組織資源](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [如何透過電子郵件要求 Azure 發票的副本](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [如何從 Azure 新增、更新或移除信用卡或付款卡](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [管理 (重新啟用/取消/切換) 訂閱](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



