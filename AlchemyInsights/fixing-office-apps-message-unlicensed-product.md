---
title: 無法啟用 Office
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
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327837"
---
# <a name="unable-to-activate-office"></a>無法啟用 Office

**請注意**：如果您使用舊版 Windows，請確認 TLS 1.2 已預設啟用 (例如，Windows 7)。 如需詳細資訊，請參閱 [更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

- 檢查您的訂閱狀態是否已過期。
- 確認您擁有允許用戶端授權的訂閱 (例如 Office 365 商務版或商務進階版)，並[確保該使用者已獲派授權](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)。
- 請確認使用者使用所指派授權的相同帳戶登入 Office。
- 查看 [Office 365 服務健康情況頁面](https://docs.microsoft.com/office365/enterprise/view-service-health)，以查看服務是否有任何已知問題。
- 檢查您的防火牆、防毒軟體和 Proxy 設定，確認未封鎖 Microsoft 365 應用程式存取網際網路。請參閱 [Office 365 URL 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 和 IP 位址範圍")。

**提示**：在 Windows 電腦上，我們可以為您診斷並自動修正數種常見的 Office 登入問題。 下載並執行 **[Microsoft 支援及修復小幫手](https://aka.ms/SaRA-OfficeSignInScenario)** 以使用我們的自動化工具。

請使用下列疑難排解動作：

- 開啟 Office App，並 [[登出]](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何現有的使用者帳戶。 [[移除]](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 並 [[重新指派]](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office 授權，然後使用受影響的使用者帳戶 [[登入 Office]](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。
- 執行 [[啟用疑難排解員]](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [重設 Office 啟用狀態](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "重設 Office 啟用狀態")
- [執行 Office 線上修復](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

如需其他疑難排解解決方案，請參閱：  

- [Office 中的「未授權產品」及啟用錯誤](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [啟用 Office 時，「很抱歉，我們無法連線至您的帳戶。請稍後再試一次」的錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)