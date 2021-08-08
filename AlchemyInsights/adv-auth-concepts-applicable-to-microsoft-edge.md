---
title: 適用于 Microsoft Edge 的高級驗證概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934356"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>適用于 Microsoft Edge 的高級驗證概念

以下是適用于 Microsoft Edge 的高級驗證概念：

**主動驗證**

當您啟用[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621)原則時，Microsoft Edge 會嘗試透過 Microsoft 服務主動驗證已登入的使用者。 以固定的間隔，它會使用線上服務檢查是否有包含管理主動驗證的更新資訊清單。

好處：主動型驗證可讓驗證重要服務，例如 Office 新的] 索引標籤頁面。 此外，如果使用 Bing 做為搜尋引擎，事前驗證會提升位址列的效能，並可協助產生針對您的業務需求個人化的搜尋結果。

**Windows Hello用於 NTLM 驗證的 CredUI**

若在網站嘗試透過 NTLM 或協商機制登入使用者時，無法使用單一登入 (SSO) ，這項功能可讓使用者與網站共用作業系統認證，並使用 Windows Hello 身分驗證 UI 來滿足驗證質詢。 此登入流程只會出現在 Windows 10，而且只適用于在 NTLM 或協商質詢期間未取得 SSO 的使用者。

**使用儲存的密碼自動登入**

在 Microsoft Edge 中儲存密碼的使用者可以啟用自動登入已儲存認證的網站。 使用者可以在 edge://settings/passwords 中開啟或關閉此功能，也可以在 [密碼管理員](https://go.microsoft.com/fwlink/?linkid=2134622) 原則中加以設定。
