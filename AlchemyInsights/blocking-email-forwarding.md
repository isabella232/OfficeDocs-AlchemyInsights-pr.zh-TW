---
title: 726封鎖電子郵件轉發
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478312"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="3f732-102">封鎖或取消封鎖電子郵件轉發</span><span class="sxs-lookup"><span data-stu-id="3f732-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="3f732-103">若要啟用或停用特定信箱的電子郵件轉寄功能，請參閱 [設定電子郵件轉接](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="3f732-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="3f732-104">在租使用者層級上，會使用輸出垃圾郵件原則來控制外部轉送。</span><span class="sxs-lookup"><span data-stu-id="3f732-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="3f732-105">您可以從 [這裡](https://protection.office.com/antispam) 的安全性與合規性中心檢查輸出垃圾郵件篩選原則，或使用 [Get-HostedOutboundSpamFilterPolicy 命令](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)。</span><span class="sxs-lookup"><span data-stu-id="3f732-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="3f732-106">如果您收到下列錯誤：「 **550 5.7.520 存取權遭到拒絕，您的組織不允許外部轉送**」，請確定原則已設定為啟用外部自動轉寄。</span><span class="sxs-lookup"><span data-stu-id="3f732-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="3f732-107">**附注：** 建議您在預設的輸出垃圾郵件篩選原則上停用外部 Autoforward，並僅針對需要外部轉寄的使用者，為這些使用者建立自訂原則加以啟用。</span><span class="sxs-lookup"><span data-stu-id="3f732-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="3f732-108">您可以在 Office 365 中深入瞭解設定 [外部電子郵件](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)轉寄。</span><span class="sxs-lookup"><span data-stu-id="3f732-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>