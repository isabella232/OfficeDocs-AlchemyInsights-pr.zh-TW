---
title: 在 Microsoft 365 應用程式中登入的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744623"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>簽入 Microsoft 365 Apps 的問題

附注：如果您使用的是舊版本的 Windows (例如 Windows 7 SP1、Windows Server 2008 R2) ，請使用[簡易修正](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)，將 TLS 1.2 啟用為預設值。 如需詳細資訊，請參閱 [更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

若要修正 Microsoft 365 應用程式的登入問題，請嘗試在受影響電腦上執行下列選項：  

- 如 Windows 所述，請參閱[解決常見登入問題的建議](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- 若為 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**提示**：在 Windows 電腦上，我們可以為您診斷並自動修正數種常見的 Office 登入問題。 下載並執行 **[Microsoft 支援及修復小幫手](https://aka.ms/SaRA-OfficeSignInScenario)** 以使用我們的自動化工具。

**附注：** 停用新式驗證 (ADAL) 或網頁帳戶管理 (WAM) 以修正登入或啟用問題  **，不建議使用此選項**。 如果使用 Office 2013 連接至 Microsoft 365 時發生錯誤，請確定您為 Office 用戶端[啟用新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。

如需特定疑難排解動作，請參閱：

[在 Windows 10 上更新至 Office 2016 組建 16.0.7967 之後，在登入時發生連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[您無法登入您的組織帳戶，例如 Office 365、Azure 或 Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[如何疑難排解無法登入 Office 365、Azure 或 Intune 的非瀏覽器應用程式](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[在 Office 中重複提示認證](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)