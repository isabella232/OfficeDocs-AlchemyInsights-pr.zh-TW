---
title: 緩解未偵測到應用程式的錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810475"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>緩解「未偵測到應用程式」的錯誤

在所有主要的 OS 平台 (Windows、iOS 和 Android) 上，都可能發生由 Intune 回報的應用程式安裝錯誤：「未偵測到成功完成安裝後的應用程式」。

最常產生此錯誤的情況包括：

- 初次部署之後，應用程式在 Intune 外部 (從第三方應用程式商店) 進行更新。 例如，某些應用程式 (例如 Google Chrome) 可能會執行自動更新。
- 初次安裝後，使用者將應用程式解除安裝。

若要緩解此問題，請先檢查受影響的裝置，以判斷發生錯誤的情形。

- 如果應用程式已於 Intune 外部更新，可以將應用程式部署設定為忽略應用程式版本。 若要這麼做，請在 [應用程式設定] > [應用程式資訊]**** 底下，將 [忽略應用程式版本]**** 設為 [是]****。
- 若以用戶端為目標，建議您將應用程式部署為「必要」，並確定部署的是最新版本。
- 或者，在 iOS 平台上，您可以使用與 Apple 大量採購方案 (Volume Purchase Program) 關聯的**自動更新**功能，以設定為在新應用程式版本推出時自動更新。

如需針對應用程式安裝問題進行疑難排解的詳細資訊，請參閱[針對應用程式安裝問題進行疑難排解](https://docs.microsoft.com/intune/troubleshoot-app-install)。
