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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449084"
---
# <a name="password-synchronization"></a>密碼同步處理

**密碼雜湊同步處理完全無法運作**

當密碼雜湊同步處理無法運作時，客戶遇到的一些常見問題包括：

- Azure AD Connect 所使用的 Active Directory 帳戶不會被授與內部部署 Active Directory 的「 **複製目錄變更** 」和「複寫 **目錄變更」所有** 許可權（密碼同步處理所需）。您必須將這些許可權授與 Active Directory 帳戶，以修正此問題。
- 在管理員將使用者 Sign-In 方法從 [ **密碼同步** 處理] 變更為另一個選項（例如，Azure ad connect 嚮導中的 [ **同盟與 AD FS** ]）之後，就會停用密碼雜湊同步處理。您可以在 azure ad connect 嚮導中重新啟用 **密碼雜湊同步** 處理功能，以修正此問題。
- 內部部署 Active Directory 的連線問題。 例如，有些網域控制站無法透過 Azure AD Connect 存取，或防火牆已封鎖 [所需的埠](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) -您必須確保 Azure AD Connect 伺服器與內部部署 Active Directory 之間的連線能夠正常運作，以修正此問題。
- Azure AD Connect 伺服器目前處於過渡模式，這會導致伺服器無法進行密碼雜湊-若要疑難排解問題，請遵循 section [使用 AZURE AD Connect sync 的密碼同步處理疑難排解](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)一節所述的步驟進行。不會同步處理密碼。

**密碼雜湊同步處理不適用於某些使用者**

1. 如果您注意到密碼雜湊未同步處理使用者，請使用 Azure AD Connect 中的 **疑難排解** 工作進行調查並解決問題。 請執行下列工作：

    a. [在嚮導中執行疑難排解工作](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [使用疑難排解 Cmdlet 調查特定用途的密碼雜湊同步處理問題](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. 已啟用 **[使用者必須在下次登入時變更密碼]** 選項的內部部署 Active Directory 使用者物件。 當此選項啟用時，使用者會被指派臨時密碼，並會在下次登入時提示您變更密碼。 Azure AD Connect 不會將臨時密碼同步處理到 Azure AD。

若要解決上述問題，請執行下列其中一項工作：

- 請使用者登入內部部署應用程式 (例如，Windows 桌面) 並變更密碼。 新密碼會同步處理至 Azure AD。
- 讓管理員更新使用者的密碼，而不啟用 [ **使用者必須在下次登入時變更密碼]**，並與使用者共用新密碼。

3. **未正確設定** 內部部署 Active Directory 使用者物件，以進行物件同步處理或密碼同步處理。 若要解決此問題，請遵循 [使用 AZURE AD Connect Sync 疑難排解密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)中所述的步驟。







