---
title: 使用 Intune 傳送自訂通知
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086155"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>如何將自訂通知傳送給受管理的 iOS 和 Android 裝置的使用者

使用者裝置上的公司入口網站應用程式會處理 Intune 的自訂通知。 然後，應用程式會在該裝置上建立推播通知。

以下是支援接收自訂通知的裝置必要條件，然後讓應用程式建立推播通知：

- 裝置必須已安裝公司入口網站應用程式。  

- 裝置必須允許公司入口網站的應用程式傳送推播通知。 安裝或更新應用程式時，會提示使用者允許通知。

- Android 裝置必須已安裝 Google Play 服務。

- 裝置必須使用 Intune 註冊。

如需詳細資訊，包括如何傳送郵件，請參閱 [功能檔](https://docs.microsoft.com/intune/custom-notifications)。
