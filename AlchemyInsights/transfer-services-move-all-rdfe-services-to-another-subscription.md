---
title: 傳輸服務-將所有 RDFE 服務移至另一個訂閱
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681460"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>傳輸服務-將所有 RDFE 服務移至另一個訂閱

**移動資源**

Azure 資源可使用 Azure 入口網站、Azure PowerShell、Azure CLI 或 REST API 移至相同訂閱下的其他 Azure 訂閱或資源群組，以移動資源。

您可以移動資源之前，請參閱：

- [移動資源前的檢查清單](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [可以移動的服務](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [如何驗證移動](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [服務的移動指導方針](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

若要將現有資源移至另一個資源群組或訂閱，您可以使用：

- [Azure 入口網站](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

教程： [將 Azure 資源移至另一個資源群組或訂閱](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**疑難排解 Azure 資源管理員的錯誤**

請參閱下列文章，以瞭解一些常見的 Azure 部署錯誤，並收到資訊以加以解決。 如果您找不到您的部署錯誤的錯誤碼，請參閱 [find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)。

- [疑難排解部署錯誤](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [疑難排解將 Azure 資源移至新的資源群組或訂閱](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

請注意，如果您想要升級您的 Azure 訂閱，例如從空閒切換成隨移即付即用，您必須轉換您的訂閱。

- 若要升級免費試用版，請參閱將 [您的免費試用版或 Microsoft 想像 Azure 訂閱升級為隨需付費](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)。
- 若要變更隨用付費帳戶，請參閱將您的 [Azure 隨付即用訂閱變更為不同的服務](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)。

**若要將 Azure 訂閱新增或關聯至您的 Azure Active Directory 租使用者：**

1. 從 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)中的 [訂閱] 頁面登入並選取您要使用的訂閱。
2. 選取 [ **變更目錄**]。
3. 查看顯示的任何警告，然後選取 [ **變更**]。
4. 訂閱已變更目錄，您會收到一則成功的訊息。
5. 使用 *目錄* 切換器移至新目錄。 最多可能需要10分鐘的時間，才能正確顯示所有專案。

**建譯的文件**

- [轉移 Azure 訂閱的擁有權](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [將資源移至新的資源群組或訂閱](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [使用 Azure 入口網站管理資源](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
