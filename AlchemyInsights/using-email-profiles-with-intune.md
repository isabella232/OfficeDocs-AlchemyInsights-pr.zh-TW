---
title: 使用 Intune 電子郵件設定檔
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653279"
---
# <a name="using-email-profiles-with-intune"></a>使用 Intune 電子郵件設定檔

您可使用 Intune 在多個裝置平台上建立並部署本機 (內建 ) 電子郵件用戶端的電子郵件設定檔。

關於電子郵件設定檔相關的某些限制的資訊 (包括如何處理現有設定檔的顯示狀態，以及如何移除電子郵件設定檔)，請參閱[使用 Intune 新增電子郵件設定到裝置](https://docs.microsoft.com/intune/email-settings-configure)。

有關如何為每個裝置平台建立電子郵件設定檔的詳細資訊，請參閱：

[Android 裝置設定在 Intune 中設定電子郵件、驗證和同步](https://docs.microsoft.com/intune/email-settings-android)  
[iOS 和 iPadOS 裝置在 Microsoft Intune 中新增電子郵件設定](https://docs.microsoft.com/intune/email-settings-ios)  
[執行 Windows Phone 8.1 的裝置在 Microsoft Intune 中的電子郵件設定檔設定。](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[執行 Windows 10 的裝置在 Microsoft Intune 中的電子郵件設定檔設定](https://docs.microsoft.com/intune/email-settings-windows-10)

**常見的同步問題**

**Android 電子郵件設定檔上的 KNOX 可防止使用者的連絡人、行事曆及工作同步至使用者裝置。**

Android KNOX 電子郵件設定檔上的 KNOX 提供管理員通過啟要同步的內容類型來決定要將哪些內容類型同步處理到裝置的選項。

如果任何內容類型的被設定為**未設定** (預設)，該內容類型就不會自動同步。 使用者可以直接在裝置上手動啟用所需的內容類型，但該設定會被 Intune 原則設定所覆寫，並且該內容類型的同步將停止。

