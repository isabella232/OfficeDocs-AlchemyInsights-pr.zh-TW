---
title: 密碼原則
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040821"
---
# <a name="password-policies"></a>密碼原則

**我在使用使用者的密碼原則時發生問題**

- 使用者的密碼原則取決於使用者是否僅限雲端或內部部署。
- 僅限雲端使用者必須選擇符合本文中需求的密碼： [僅適用于雲端使用者帳戶的密碼原則](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- 內部部署使用者必須選擇符合內部部署需求的密碼。 如果內部部署使用者無法設定其密碼，請檢查您的內部部署需求。

**我不知道如何設定或檢查密碼到期原則**

- 您可以使用 PowerShell 來設定及檢查您租使用者中的雲端使用者到期原則。 遵循本文中的指示： [使用 PowerShell 設定或檢查密碼原則](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- 內部部署使用者的密碼到期原則是在您的內部部署 AD 中設定。

**其他有用的連結：**
- [密碼重設入門](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [疑難排解管理員初始化的密碼重設](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
