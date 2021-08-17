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
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107150"
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
 
若要深入了解使用 Microsoft 365 轉送電子郵件的選項和步驟，請參閱[如何將多功能裝置或應用程式設定為使用 Microsoft 365 或 Office 365 傳送電子郵件](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。