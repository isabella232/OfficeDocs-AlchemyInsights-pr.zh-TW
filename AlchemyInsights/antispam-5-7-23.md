---
title: 反垃圾郵件-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717316"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="95652-102">修正錯誤碼為5.7.23 的電子郵件傳遞問題</span><span class="sxs-lookup"><span data-stu-id="95652-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="95652-103">在 web 上公開提供的 SPF 或 DNS 記錄檢查，確認您網域的 SPF DNS 記錄。</span><span class="sxs-lookup"><span data-stu-id="95652-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="95652-104">確認輸出郵件未被 Microsoft 識別為垃圾郵件，並透過 [高風險傳遞集](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)區路由傳送。</span><span class="sxs-lookup"><span data-stu-id="95652-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="95652-105">高風險傳遞集區中的郵件不會通過 SPF 檢查，因此目的地電子郵件組織不會接受此項功能。</span><span class="sxs-lookup"><span data-stu-id="95652-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="95652-106">如果問題持續發生，您可能需要與您嘗試傳送電子郵件的郵件主機系統管理員聯繫。</span><span class="sxs-lookup"><span data-stu-id="95652-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="95652-107">請記下退回郵件中提供的詳細外部錯誤。</span><span class="sxs-lookup"><span data-stu-id="95652-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="95652-108">Microsoft 支援部門可能無法進一步協助。</span><span class="sxs-lookup"><span data-stu-id="95652-108">Microsoft support may not be able to assist further.</span></span>
