---
title: 關於 Yammer 中的身分識別
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664161"
---
# <a name="about-identity-in-yammer"></a>關於 Yammer 中的身分識別

建議所有網路採取以下步驟，以避免身分識別相關問題:

1. 在 Azure AD 中為使用者提供 Microsoft 365 帳戶後，強制執行 Office 365 身分識別，以確保所有使用者都使用自己的主要 Microsoft 365 帳戶登入。 如需詳細資訊，請參閱 [針對 Yammer 使用者強制執行 Office 365 身分識別](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。
2. 合併多個 Yammer 網路。 舊版 Yammer 設定允許多個 Yammer 網路連線到一個租使用者。 如需詳細資訊，請參閱[網路移轉 - 合併多個 Yammer 網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。
3. 您也可以選擇強制執行 Yammer 授權，以封鎖 Yammer 中沒有授權的使用者。 如需詳細諮詢，請參閱 [在 Office 365 中管理 Yammer 使用者授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)。
4. 最後，稽核之前的 Yammer 網路使用者清單，並暫停舊版使用者。 建議您暫停（停用）使用者，而不是刪除使用者，因為刪除操作不可逆。 如需詳細資訊，請參閱[稽核已連結至 Office 365 網路的 Yammer 使用者](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)，並[移除使用者](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。

透過使用下列步驟來設定 Yammer，您也可以準備將 您的 Yammer 網路設定為適用於 Microsoft 365 的原生模式。 如需詳細資訊，請參閱 [針對適用於 Microsoft 365 的原生模式設定您的 Yammer 網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)。