---
title: 2491警示來自「由於租使用者或使用者覆寫」原則，來自網路釣魚傳遞的電子郵件訊息
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728602"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>警示來自「由於租使用者或使用者覆寫」原則，來自網路釣魚傳遞的電子郵件訊息

名為 "由於租使用者或使用者覆寫，已將「網路釣魚已傳送」的預設警示原則，已向租使用者提供 Office 365 ATP P1 和 P2 授權。 如果您收到此警示，請參閱下列步驟：

1. 從警示訊息中，按一下 [ **查看警示** ]，以移至安全性 & 規範中心中的 [ **警示** ] 頁面。

2. 選取 [警示]，以查看在**瀏覽器中****查看訊息清單**或查看訊息的選項。 這兩個選項都會帶您前往郵件的詳細資料，其中包含郵件識別碼。 請注意，威脅瀏覽器連結將會自動篩選符合警示準則的郵件。 您可能需要在威脅瀏覽器中調整日期篩選器。

由於手動設定的覆寫，所以已傳遞網路釣魚郵件：

- 由使用者設定的允許寄件者或網域。

- 反垃圾郵件原則中由系統管理員設定的允許寄件者或網域。

- 連線篩選原則中的允許 IP 位址。

- 郵件流程規則 (也稱為已設定為允許郵件的傳輸規則) 。

如果您認為郵件已錯誤標示為網路釣魚，請使用 Outlook [報告訊息增益集](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) 將郵件範例提交給 Microsoft。
