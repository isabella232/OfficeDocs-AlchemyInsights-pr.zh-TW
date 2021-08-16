---
title: 重設密碼時的問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039957"
---
# <a name="problems-resetting-password"></a>重設密碼時的問題

以下是重設密碼及可能的解決方案時可能面臨的一些問題：

**我遇到其他類別未涵蓋的密碼重設問題**

- 確定您有權重設密碼。 只有全域、密碼和使用者管理員才能重設使用者密碼。 全域管理員也可以重設其他特權管理員的密碼。
- 確定您瞭解授權需求：
    - 您的組織中必須至少有一個指派的授權
        - 僅限雲端使用者-任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic
        - 雲端和/或內部部署使用者-Azure AD Premium P1 或 P2、Enterprise Mobility + Security (EMS) 或 Secure Productive Enterprise (SPE) 
        - 若要閱讀授權要求的詳細資訊，請參閱 [Microsoft AZURE AD 自助密碼重設的授權需求一](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)文。

**我在測試設定的密碼重設原則時發生問題**

- 最近套用的原則可能需要數分鐘的時間才能跨所有資料中心和端點進行複製。 從資料中心的實體距離也會影響套用變更的速度。
- 與使用者進行測試，而不是以系統管理員的身分進行測試，而是一小組使用者的試驗。 在 Azure 入口網站中設定的原則只適用于使用者，而非系統管理員。 Microsoft 對任何 Azure 系統管理員角色強制實施強預設雙門密碼重設原則 (例如：全域系統管理員、服務台管理員、密碼管理員等 ) 
    - 深入瞭解系統 [管理員的原則](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)。

**我想要部署密碼重設，但不想讓使用者註冊其他安全性資訊**

預先填入使用者的資料，使其不需要！ -以系統管理員的身分，您可以設定使用者的電話和電子郵件內容，然後再將密碼重設為您的組織。 您可以使用 API、PowerShell 或 Azure AD 連線來執行此動作。 其他資訊：
- [部署密碼重設，但不需要使用者註冊](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [密碼重設所使用的資料](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**[密碼重設] 按鈕會灰顯**

您未獲授權，無法重設此使用者的密碼。 只有全域、密碼和使用者管理員才能重設使用者密碼。 全域管理員也可以重設其他特權管理員的密碼。

**我沒有看到密碼重設的刀片式伺服器**

您未獲授權，無法重設密碼。 只有全域、密碼和使用者管理員才能重設使用者密碼。 全域管理員也可以重設其他特權管理員的密碼。

**在密碼重設中看不到內部部署整合刀片式伺服器**

- 內部部署整合刀片式伺服器只會出現在混合環境中，也就是說，您使用密碼寫回來處理內部部署使用者的密碼。
- 在下列情況中看不到此邊欄：
    - 您不是使用密碼回寫
    - 密碼寫回的安裝/連線發生問題
    - Azure AD 連線的安裝/連線能力有問題
    - 如需有關密碼寫回問題的疑難排解步驟，請參閱[密碼寫回疑難排解](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)一節。

**我不知道如何重設使用者的密碼**

1. 以適當的系統管理員身分登入 Azure 入口網站。
1. 移至 [使用者和群組] 邊欄，選取 [ **所有使用者**]。
1. 從清單中選取使用者。
1. 針對選取的使用者，選取 **[概述**]，然後在命令列中，按一下 [ **重設密碼**]。
1. 依照畫面上的指示進行。
    - 僅透過 Azure 入口網站支援密碼回寫進行重設。

**我從 Office 365 系統管理員入口網站或 Office 365 行動應用程式重設內部部署使用者的密碼，但使用者仍無法登入**

此入口網站不支援密碼回寫。 在 Azure 入口網站中重新重設使用者的密碼 portal.azure.com

