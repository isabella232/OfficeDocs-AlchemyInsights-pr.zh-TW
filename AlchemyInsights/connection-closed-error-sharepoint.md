---
title: SharePoint 中的基礎連線已關閉錯誤
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044403"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>SharePoint 中的「基礎連線已關閉」錯誤

如果您在 SharePoint 中收到「基礎連線已關閉」錯誤，它可能和 TLS 1.0/1.1 的淘汰有關。如需詳細資訊，請參閱這些文章：

- [在 Office 365 和 Office 365 GCC 中準備 TLS 1.2](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [如果用戶端沒有 TLS 1.2 支援，則會發生驗證錯誤](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

若使用者使用的是 Windows 7，請確保他們檢查 [Windows 7 中的 TLS 加密套件](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。