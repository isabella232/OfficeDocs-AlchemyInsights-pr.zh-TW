---
title: 解決 Teams 登入錯誤 AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687029"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>解決 Teams 登入錯誤 AADSTS9000411

當登入 Microsoft Teams 時，您可能會收到以下錯誤：[很抱歉，我們無法將您登入 AADSTS9000411: 要求的格式不正確。參數 "login_hint" 重複。]****

若要解決此問題，請確認您的 Microsoft Teams 用戶端已更新。 如需更新用戶端的詳細資訊，請參閱[更新 Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

如果您因為某些原因而無法更新用戶端，登出用戶端將清除大部分的快取資料。 不過，如果您在登出/登入後仍有問題，請結束 Teams，並執行下列動作清除用戶端快取：
1. 關閉 Microsoft Teams。
2. 移至：%appdata%\microsoft\teams 並刪除所有檔案。
3. 重新開啟 Microsoft Teams。
