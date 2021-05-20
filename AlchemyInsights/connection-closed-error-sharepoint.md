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
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543028"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="95680-102">SharePoint 中的「基礎連線已關閉」錯誤</span><span class="sxs-lookup"><span data-stu-id="95680-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="95680-p101">如果您在 SharePoint 中收到「基礎連線已關閉」錯誤，它可能和 TLS 1.0/1.1 的淘汰有關。如需詳細資訊，請參閱這些文章：</span><span class="sxs-lookup"><span data-stu-id="95680-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="95680-105">在 Office 365 和 Office 365 GCC 中準備 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="95680-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="95680-106">如果用戶端沒有 TLS 1.2 支援，則會發生驗證錯誤</span><span class="sxs-lookup"><span data-stu-id="95680-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="95680-107">更新以在 Windows 版 WinHTTP 中啟用 TLS 1.1 和 TLS 1.2 做為預設安全通訊協定</span><span class="sxs-lookup"><span data-stu-id="95680-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="95680-108">若使用者使用的是 Windows 7，請確保他們檢查 [Windows 7 中的 TLS 加密套件](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。</span><span class="sxs-lookup"><span data-stu-id="95680-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>