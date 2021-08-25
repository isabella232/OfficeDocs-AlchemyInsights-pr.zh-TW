---
title: 停用 TLS 1.0 和 TLS 1.1 進行 SMTP 驗證用戶端提交
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/18/2021
ms.locfileid: "58380668"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>停用 TLS 1.0 和 TLS 1.1 進行 SMTP 驗證用戶端提交

我們最近已開始停用 SMTP 驗證用戶端提交的 TLS 1.0 和 TLS 1.1。 

如果您已將裝置、應用程式或伺服器設定為使用 SMTP 驗證用戶端提交方法，將電子郵件傳送至 Microsoft 365，請確定您的裝置、應用程式或伺服器都支援適用於 SMTP 的 TLS 1.2。 