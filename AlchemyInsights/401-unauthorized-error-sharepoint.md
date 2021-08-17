---
title: SharePoint 中的 401 未授權錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314339"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>SharePoint 中的 401 未授權錯誤

如果您在 SharePoint 中收到「(401) 未授權」錯誤，這可能與 TLS 1.0/1.1 的淘汰有關。如需詳細資訊，請參閱：

- [在 Office 365 和 Office 365 GCC 中準備 TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [如果用戶端沒有 TLS 1.2 支援，則會發生驗證錯誤](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

若使用者使用的是 Windows 7，請確保他們檢查 [Windows 7 中的 TLS 加密套件](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。