---
title: AAD 連線健康情況的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923743"
---
# <a name="problem-with-aad-connect-health"></a>AAD 連線健康情況的問題

- 確定您有權執行此作業。 全域管理員預設可以存取。 此外，您可以使用 [角色型存取控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) ，將註冊許可權委派給投稿者。
- 確定所需端點已啟用，但由於防火牆而未封鎖。 如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。
- 因為網路層對 SSL 檢查進行的輸出通訊，所以註冊可能會失敗。
- 請確認您已驗證 Azure AD 連線健康狀態的通知設定。 請複查您的設定。 本[指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)可協助您瞭解如何設定 Azure AD 連線狀況通知的通知設定。
- 若要深入瞭解 AAD 連線健康情況同步處理報告以及如何下載它，請參閱[物件層級同步處理報告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。

若要疑難排解 AAD 連線狀況警示，請遵循[有關 aad 連線 Health data freshness alerts 的疑難排解指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)和常見問題，請參閱[常見 AAD 連線健全性安裝問題](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。
