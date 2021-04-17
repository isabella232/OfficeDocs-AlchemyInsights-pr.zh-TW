---
title: 轉移 Azure 帳單擁有權
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
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820601"
---
# <a name="transfer-azure-billing-ownership"></a>轉移 Azure 帳單擁有權

以擁有要轉移的訂閱的計費帳戶的管理員身份登入到 [Azure 入口網站](https://portal.azure.com/)。 如果不確定您是否是管理員，或者您需要確定是誰，請參閱[確定帳戶計費管理員](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)。

1. 搜尋 _成本管理 + 計費_。
1. 從左方窗格中選取 **訂閱**。 依據存取權而定，您可能需要選取計費範圍，然後 **訂閱** 或 **Azure 訂閱**。
1. 針對您想要轉移的訂閱，選取 **[轉移帳單擁有權]**。
1. 輸入使用者的電子郵件地址，其為訂閱的新擁有者帳戶的計費管理員，然後選取 **傳送轉移要求**。
1. 使用者會收到一封電子郵件，其中包含檢閱您的轉移要求的指示。 若要核准轉移要求，使用者會選取電子郵件中的連結，並遵循指示操作。

請注意，如果您將您的訂閱帳單擁有權轉移至另一個 Azure AD 租用戶的使用者帳戶，在訂閱中用以管理資源的所有 [角色型存取控制 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 作業皆會永久移除。 只有新擁有者才有權管理訂閱中的資源。 如需關於如何變更訂閱目錄的詳細資訊，請參閱 [將訂閱轉移到另一個 Azure AD 租用戶中的使用者](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。

_**您發票上的重要影響**_：如果您已轉移 Azure 訂閱的帳單擁有權，您將會以估價計費。 您可以按照下列步驟存取發票：  

1. 以  [有權存取發票的使用者](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) 之身分，在 Azure 入口網站的  [[訂閱] 頁面](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 中選取您的訂閱，然後選取  **[發票]**。
1. 按一下  **[下載發票]**  以查看您的 PDF 發票複本。 如果顯示  _[無法使用]_，請查閲 [為什麼我看不到上一個計費期間的發票？](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)。
1. 您也可以按一下 **計費期間** 來檢視您的每日使用情況 要取得發票的 PDF 和詳細的日常使用量檔案 (.CSV) 的副本。 如需詳細資訊，請參閱 [取得發票和使用狀況資料](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)。

**建議的文件**

- [轉移 Azure 訂閲帳單擁有權到另一個帳戶](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [關於轉移 Azure 訂閱的帳單擁有權](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [傳送 Visual Studio、Microsoft 合作夥伴網路 (MPN) 和 [預付方案] 開發/測試訂閱](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [轉移擁有權常見問題](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [轉移擁有權問題的疑難排解](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
