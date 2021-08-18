---
title: Microsoft 365 郵件服務的 SMTP 設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: e4d16a8d04b4d2fb4bfa8cf84308e29f2b499e0680f656cc239411d06e5b077c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900867"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Microsoft 365 郵件服務的 SMTP 設定

以下是 Microsoft 365 郵件服務的 SMTP 設定：

**伺服器**：smtp.office365.com </br>
**連接埠**：587 </br>
**加密**：STARTTLS (目前僅支援 TLS 1.2 版本。 請確定您的應用程式或裝置支援 TLS 1.2) </br>
**使用者名稱**：您的 Office 365 地址 (例如 example@yourdomain.com) </br>
**密碼**：您的 Office 365 密碼 </br>
**驗證**：必要的 </br>
**傳送限制**：每天 10,000 封電子郵件 </br>

如需 POP 和 IMAP 設定，請參閱 [POP、IMAP 和 SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)。
 
若要深入了解使用 Microsoft 365 轉送電子郵件的選項和步驟，請參閱[如何將多功能裝置或應用程式設定為使用 Microsoft 365 或 Office 365 傳送電子郵件](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。