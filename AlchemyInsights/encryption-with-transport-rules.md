---
title: 使用傳輸規則加密
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915044"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="16c5f-102">使用傳輸規則加密</span><span class="sxs-lookup"><span data-stu-id="16c5f-102">Encryption with transport rules</span></span>

<span data-ttu-id="16c5f-103">在 [Exchange 系統管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，您可以在郵件流程規則中使用 Office 郵件加密 (OME) 功能來觸發郵件加密。</span><span class="sxs-lookup"><span data-stu-id="16c5f-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="16c5f-104">在 [傳出規則] 條件上選擇 [套用 Office 365 郵件加密與權限保護]\*\*\*\* 選項。</span><span class="sxs-lookup"><span data-stu-id="16c5f-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="16c5f-105">如需詳細資訊，請參閱[定義郵件流程以進行加密](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。</span><span class="sxs-lookup"><span data-stu-id="16c5f-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="16c5f-106">在 Powershell 中，使用 [TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) Cmdlet，並將 *ApplyOME* 參數設為 $true。</span><span class="sxs-lookup"><span data-stu-id="16c5f-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
