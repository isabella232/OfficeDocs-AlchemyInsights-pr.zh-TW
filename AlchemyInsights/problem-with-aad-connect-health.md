---
title: AAD Connect Health 的問題
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453289"
---
# <a name="problem-with-aad-connect-health"></a>AAD Connect Health 的問題

- 確定您有權執行此作業。 全域管理員預設可以存取。 此外，您可以使用 [角色型存取控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) ，將註冊許可權委派給投稿者。
- 確定所需端點已啟用，但由於防火牆而未封鎖。 如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。
- 因為網路層對 SSL 檢查進行的輸出通訊，所以註冊可能會失敗。
- 請確認您已驗證 Azure AD Connect Health 的通知設定。 請複查您的設定。 本 [指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) 可協助您瞭解如何設定 Azure AD Connect health 通知的通知設定。
- 若要深入瞭解 AAD Connect Health sync 報表及如何下載它，請參閱 [物件層級同步處理報告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。

若要疑難排解 AAD Connect 狀況警示，請遵循 [Aad Connect health 資料新鮮度警示的疑難排解指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 及常見問題的疑難排解，請參閱 [常見的 AAD connect Health 安裝問題](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。
