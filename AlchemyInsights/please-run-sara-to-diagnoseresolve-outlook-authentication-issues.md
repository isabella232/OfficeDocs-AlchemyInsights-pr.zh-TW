---
title: 182請執行 SaRA 以診斷及解決 Outlook 驗證問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802012"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="08f1c-102">使用 SaRA 來診斷和解決 Outlook 驗證問題</span><span class="sxs-lookup"><span data-stu-id="08f1c-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="08f1c-103">**附注**：請查看是否已為您的組織啟用 [安全性預設值](https://aka.ms/securitydefaults) 。</span><span class="sxs-lookup"><span data-stu-id="08f1c-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="08f1c-104">如果您的租使用者在2019年10月21日之後建立，且您的 Outlook 不斷要求您輸入密碼，您可能會在您的租使用者中啟用 **安全性預設值** 。</span><span class="sxs-lookup"><span data-stu-id="08f1c-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="08f1c-105">我們強烈建議您使用 [outlook 繼續要求我的密碼](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) 診斷在受影響的機器上進行疑難排解，以疑難排解 outlook 不斷提示密碼的問題。</span><span class="sxs-lookup"><span data-stu-id="08f1c-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="08f1c-106">此 [SaRA](https://diagnostics.office.com/#/) 診斷會執行自動化檢查，並傳回可能的解決方案，讓您用來處理任何偵測到的問題。</span><span class="sxs-lookup"><span data-stu-id="08f1c-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
