---
title: 密碼同步處理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960826"
---
# <a name="password-synchronization"></a>密碼同步處理

**密碼雜湊同步處理完全無法運作**

當密碼雜湊同步處理無法運作時，客戶遇到的一些常見問題包括：

- Azure AD 連線用於與內部部署 Active Directory 通訊的 Active Directory 帳戶，不會被授與內部部署 Active Directory 的複寫 **目錄變更** 和複寫 **目錄變更所有** 許可權（密碼同步處理所需）。您必須將這些許可權授與 Active Directory 帳戶，以修正此問題。
- 在系統管理員將使用者 Sign-In 方法從「**密碼同步** 處理」變更為另一個選項（例如，azure ad 連線中的 **AD FS 同盟**）之後，就會停用密碼雜湊同步處理。您可以在 azure ad 連線嚮導中重新啟用 **密碼雜湊同步** 處理功能，以修正此問題。
- 內部部署 Active Directory 的連線問題。 例如，有些網域控制站無法由 Azure AD 連線存取，或防火牆封鎖[所需的埠](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports)-您需要確保 azure AD 連線伺服器與內部部署 Active Directory 之間的連線正常運作。
- Azure AD 連線伺服器目前處於暫存模式，這會導致伺服器無法進行密碼雜湊-若要疑難排解問題，請遵循 section[使用 AZURE AD 的密碼同步處理疑難排解中所述的步驟連線 sync-不會同步處理任何密碼](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。

**密碼雜湊同步處理不適用於某些使用者**

1. 如果您注意到密碼雜湊未同步處理使用者，請使用 Azure AD 連線中的 **疑難排解** 工作以調查並解決問題。 請執行下列工作：

    a. [在嚮導中執行疑難排解工作](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [使用疑難排解 Cmdlet 調查特定用途的密碼雜湊同步處理問題](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. 已啟用 **[使用者必須在下次登入時變更密碼]** 選項的內部部署 Active Directory 使用者物件。 當此選項啟用時，使用者會被指派臨時密碼，並會在下次登入時提示您變更密碼。 Azure AD 連線不會將臨時密碼同步處理到 Azure AD。

若要解決上述問題，請執行下列其中一項工作：

- 請使用者登入內部部署應用程式 (例如 Windows 桌面) 和變更密碼。 新密碼會同步處理至 Azure AD。
- 讓管理員更新使用者的密碼，而不啟用 [ **使用者必須在下次登入時變更密碼]**，並與使用者共用新密碼。

3. **未正確設定** 內部部署 Active Directory 使用者物件，以進行物件同步處理或密碼同步處理。 若要解決此問題，請遵循[使用 AZURE AD 連線同步處理的疑難排解密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)中所述的步驟。







