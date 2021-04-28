---
title: Windows 7 電腦的 SharePoint 問題
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066990"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Windows 7 電腦的 SharePoint 問題

如果您在使用 SharePoint 或 OneDrive 時在 Windows 7 電腦上收到錯誤，它們可能會與 TLS 1.0/1.1 的棄用有關。 如需詳細資訊，請參閱：

- [在 Office 365 和 Office 365 GCC 中準備 TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 用戶端必須啟用 TLS1.2。 如需詳細資訊，請參閱[用戶端不具備 TLS 1.2 支援時，會發生驗證錯誤](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- 安裝 KB3140245 並建立登錄值。 如需詳細資訊，請參閱 [更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windows 7 SP1/Windows 8 用戶端必須確保已安裝最新的 TLS 加密套件。 如需詳細資訊，請參閱 [Microsoft 資訊安全摘要報告 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)。 


