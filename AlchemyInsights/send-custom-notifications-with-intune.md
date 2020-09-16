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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720637"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>如何將自訂通知傳送給受管理的 iOS 和 Android 裝置的使用者

自訂的 Intune 通知是由使用者裝置上的公司入口網站應用程式處理。 然後，應用程式會在該裝置上建立推播通知。

以下是支援接收自訂通知的裝置必要條件，然後讓應用程式建立推播通知：

- 裝置必須已安裝公司入口網站應用程式。  

- 裝置必須允許公司入口網站應用程式傳送推播通知。 安裝或更新應用程式時，會提示使用者允許通知。

- Android 裝置必須已安裝 Google Play 服務。

- 裝置必須使用 Intune 註冊。

如需詳細資訊，包括如何傳送郵件，請參閱 [功能檔](https://docs.microsoft.com/intune/custom-notifications)。
