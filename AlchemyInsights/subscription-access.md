---
title: 訂閱存取
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773770"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>因瀏覽器問題而無法登入 Azure (瀏覽器掛起、持續旋轉、未載入等等 ) 

您可能會因為中斷而受到影響。 請查看是否存在即時中斷： [Azure 健康狀態](https://status.azure.com/status/history/)。

請登出所有現用的 Azure 會話。 啟動網頁瀏覽器的內建或 incognito 模式。

您也可以嘗試重新整理瀏覽器、使用另一個瀏覽器、在上述情況下刪除快取 cookie。

深入瞭解： [疑難排解登錄問題](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**無法存取訂閱**

在 [Azure 入口網站](https://portal.azure.com/)中，確定已從右上方的帳戶選取正確的 Azure 目錄。

在 [Azure 帳戶中心](https://account.windowsazure.com/Subscriptions)，確定所使用的帳戶是否為帳戶管理員。

深入瞭解： [疑難排解未找到訂閱](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**無法存取帳單記錄**

帳戶管理員必須確定存取計費資訊的使用者已新增至 Azure Active directory，以作為來賓使用者：新增 [或刪除新使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。

然後，使用者必須具有全域系統管理員角色： [將角色指派給使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。

張貼此專案時，使用者可以使用 RBAC 原則授與存取權： [授與帳單的存取權](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)。

**建譯的文件**

-   [我無法登入以管理我的 Azure 訂閱](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)