---
title: 設定 LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090403"
---
# <a name="configure-ldap"></a>設定 LDAP

若要設定 LDAP，請執行下列操作：

1. 檢查 [Azure 入口網站](https://aka.ms/aadds-health)上網域的健康情況。
1. 請確定有效的 Azure AD 訂閱可供使用，且已啟用 Azure AD 網域服務。
1. 啟用安全 LDAP 所需的憑證必須從信任的公用憑證授權單位單位取得，或是由自我簽署的憑證取得。
1. 確定憑證遵循必要的 [指導方針](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)。

**不正確憑證**
1. 若要更新憑證，請依照下列步驟建立新的憑證和 reupload： [CONFIGURE LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。
1. 若要在 Azure Active directory 網域服務中解決安全 LDAP 警示的已知問題，請參閱 [解決 LDAP 警示](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。
