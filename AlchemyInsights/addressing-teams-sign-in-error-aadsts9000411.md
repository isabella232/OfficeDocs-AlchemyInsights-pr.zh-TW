---
title: 解決 Teams 登入錯誤 AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821978"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>解決 Teams 登入錯誤 AADSTS9000411

當登入 Microsoft Teams 時，您可能會收到以下錯誤：[很抱歉，我們無法將您登入 AADSTS9000411: 要求的格式不正確。參數 "login_hint" 重複。]

若要解決此問題，請確認您的 Microsoft Teams 用戶端已更新。 如需更新用戶端的詳細資訊，請參閱[更新 Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

如果您因為某些原因而無法更新用戶端，登出用戶端將清除大部分的快取資料。 不過，如果您在登出/登入後仍有問題，請結束 Teams，並執行下列動作清除用戶端快取：
1. 關閉 Microsoft Teams。
2. 移至：%appdata%\microsoft\teams 並刪除所有檔案。
3. 重新開啟 Microsoft Teams。
