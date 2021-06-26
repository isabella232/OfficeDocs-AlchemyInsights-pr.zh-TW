---
title: 透過 Microsoft 365 回覆電子郵件
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117974"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>設定多功能裝置或應用程式以傳送電子郵件

若要深入了解您的選項和步驟，請參閱[如何將多功能裝置或應用程式設定為使用 Microsoft 365 傳送電子郵件](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。
  
如果您的裝置或應用程式最近停止運作，最常見的問題為：

- **使用 SMTP 驗證用戶端提交時發生與驗證相關的錯誤** 我們最近做了一些與 SMTP 驗證運作方式相關的變更。 如需有關如何解決問題的詳細資訊，請參閱[修正使用 Microsoft 365 或 Office 365 傳送電子郵件的印表機、掃描器和企業營運 (LOB) 應用程式會產生的問題](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)的「驗證失敗」一節。
- **我們在與 Office 365 建立安全連線時，僅接受 TLS 1.2 版** 如果您要使用安全連線 (TLS)，請確定您的應用程式裝置支援 TLS 1.2。 如需詳細資訊，請參閱[在 Office 365 和 Office 365 GCC 中準備 TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)。
 
對於其他問題和解決方案，請參閱[修正使用 Microsoft 365 或 Office 365 傳送電子郵件的印表機、掃描器和企業營運 (LOB) 應用程式會產生的問題](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)。

若要查看受影響的裝置，請移至 [SMTP 驗證用戶端報告](https://protection.office.com/mailflow/dashboard)。

**注意**：Exchange Online 不支援大量郵寄案例。若要傳送大量商業電子郵件 (例如客戶電子報)，您應該使用專門提供這些服務的協力廠商提供者。
