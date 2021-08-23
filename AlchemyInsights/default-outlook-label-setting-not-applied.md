---
title: 未套用預設 Outlook 標籤設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370209"
---
# <a name="default-outlook-label-setting-not-applied"></a>未套用預設 Outlook 標籤設定

如果 Outlook 的預設標籤設定沒有正確套用，且有不同的標籤或沒有套用標籤，您可能會遇到已知問題 (MC277818) 而且應該執行下列兩個選項之一來解決問題：

**選項1：**

1. 請移至 Microsoft 365 規範中心 >**解決方案**  >  **資訊保護**。
1. 選取 [ **標籤原則**]，然後選取 [編輯所需的標籤原則]，以在有問題的標籤原則上沒有正確地設定 (**OutlookDefaultlabel** 設定。 執行 **labelpolicy** ，以查看此設定) ，然後選取 [ **編輯原則**]。
1. 選取 **[下一步]** ，直到您看到 [將 **此預設標籤套用至電子郵件**]，如果您在 [**原則設定**] 對話方塊中選取 [**要求使用者套用標籤來 heir 電子郵件和檔**]，便可使用此設定。
1. 在 [ **將預設標籤套用至檔** ] 對話方塊中，從下拉式清單中選擇 [ **無** ]。
1. 選取 **[下一步]** 並 **提交** ，以儲存您的標籤設定。

**選項2：**

在 [安全性與合規性中心 Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)中，使用 Set-LabelPolicy commandlet，將 {OutlookDefaultlabel = "none"} 上的 **OutlookDefaultlabel** 變更為 **None** 。

運行： `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

如需 Outlook 預設標籤的詳細資訊，請參閱[為 Outlook 設定不同的預設標籤](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)。