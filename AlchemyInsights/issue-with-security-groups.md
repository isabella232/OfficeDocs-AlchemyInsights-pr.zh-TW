---
title: 安全性群組問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925732"
---
# <a name="issue-with-security-groups"></a>安全性群組問題

**如果您收到網路錯誤 AADDS104**

不正確的網路安全性群組規則是 Azure Active Directory Domain Services (AD DS) 網路錯誤最常見的原因。 虛擬網路的網路安全性群組必須允許存取特定連接埠和通訊協定。 如果這些連接埠遭到封鎖，Azure 平台就無法監控或更新受管理的網域。 Azure AD 和 Azure AD DS 之間的同步處理也會受到影響。 請務必將預設連接埠保持開啟，以避免服務中斷。

若要瞭解並解決網路安全性群組設定問題的常見警示，請參閱[新增及驗證安全性群組](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)。
