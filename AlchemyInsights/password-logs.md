---
title: 密碼記錄檔
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960934"
---
# <a name="password-logs"></a>密碼記錄檔

**我在存取密碼重設稽核記錄檔時發生問題**

若要疑難排解存取密碼重設稽核記錄檔的問題，請執行下列步驟：

確保您獲得授權檢視稽核記錄檔。 

只有下列角色獲得授權：
 - 全域管理員
 - 安全性系統管理員
 - 安全性讀取者

**我想要查看從最初部署開始的所有密碼重設稽核事件**

過去 30 天的報告最多會儲存 120,000 個密碼重設/註冊事件。 下載 CSV 時，此上限會套用至 UI。 可透過 PowerShell 使用 1 百萬個事件。
如需詳細資訊，請參閱以下連結：

- [來自 Azure AD 報告和事件 API 的自助密碼重設事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何使用 PowerShell 快速下載密碼重設註冊事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**我想要深入瞭解有關密碼重設報告功能**

在 **使用者和群組** 下方，檢查誰在 Microsoft Azure 入口網站使用 Azure AD 密碼重設稽核記錄檔進行註冊或重設密碼。
如需詳細資訊，請參閱下列連結：

- [密碼重設報告概觀](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何在 Microsoft Azure 入口網站中檢視密碼重設報告](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [來自 Azure AD 報告和事件 API 的自助密碼重設事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [如何使用 PowerShell 快速下載密碼重設註冊事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


