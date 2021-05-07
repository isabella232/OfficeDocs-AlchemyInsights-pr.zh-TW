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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233417"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="45ccd-102">SharePoint 中的「基礎連線已關閉」錯誤</span><span class="sxs-lookup"><span data-stu-id="45ccd-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="45ccd-p101">如果您在 SharePoint 中收到「基礎連線已關閉」錯誤，它可能和 TLS 1.0/1.1 的淘汰有關。如需詳細資訊，請參閱這些文章：</span><span class="sxs-lookup"><span data-stu-id="45ccd-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="45ccd-105">在 Office 365 和 Office 365 GCC 中準備 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="45ccd-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="45ccd-106">如果用戶端沒有 TLS 1.2 支援，則會發生驗證錯誤</span><span class="sxs-lookup"><span data-stu-id="45ccd-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="45ccd-107">若使用者使用的是 Windows 7，請確保他們檢查 [Windows 7 中的 TLS 加密套件](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)。</span><span class="sxs-lookup"><span data-stu-id="45ccd-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>