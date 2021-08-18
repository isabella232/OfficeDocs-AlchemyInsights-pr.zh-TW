---
title: 網域狀態-沒有選取服務
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326568"
---
# <a name="domain-status---no-services-selected"></a>網域狀態-沒有選取服務

[**沒有選取服務**] 表示您未選取任何 Microsoft 365 服務，如 Exchange Online、商務用 Skype 或 Intune 及 Microsoft 365 的行動裝置管理，可與您的自訂網域搭配使用。 如果您使用 Exchange 混合 (Exchange 內部部署與 Exchange Online) 或外部垃圾郵件篩選使用 Exchange，但沒有其他 Microsoft 服務，您可以忽略這封郵件。 網域健康狀態僅適用于直接連線到服務的網域。

若要為您的網域選取服務：

1. 從 **設定**  >  [**網域**](https://admin.microsoft.com/Adminportal/Home)中，選取 [狀態訊息] 旁邊的網域旁邊的方塊 **未選取任何服務**。
1. 選取 [ **管理 DNS** ] 以啟動網域安裝精靈。
    - 如果您選擇 [ **新增您自己的 DNS 記錄**]，請務必在出現提示時選取服務。 其他服務可在 [ **高級選項**] 底下使用。
    - 如果您選擇 [**讓 Microsoft 新增您的 DNS 記錄** 或 **其他選項**]，請  >  **設定我的線上服務**，所有可用的服務都會受到建議並自動選取。
1. 繼續執行嚮導，以完成 DNS 安裝及服務選項。
 
如需設定網域的詳細資訊，請參閱 [新增 DNS 記錄以連接您的網域](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。

