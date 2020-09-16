---
title: 多個物件的電子郵件地址與身份識別相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724606"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="6bf4e-102">多個物件的電子郵件地址與身份識別相同</span><span class="sxs-lookup"><span data-stu-id="6bf4e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="6bf4e-103">**多個物件**</span><span class="sxs-lookup"><span data-stu-id="6bf4e-103">**Multiple objects**</span></span>

<span data-ttu-id="6bf4e-104">出現此錯誤的一個常見原因是，當多個物件的電子郵件地址與身份識別相同時，無法正確路由 Outlook Web Access 請求。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="6bf4e-105">要尋找這些物件，請運行以下命令：</span><span class="sxs-lookup"><span data-stu-id="6bf4e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="6bf4e-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="6bf4e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="6bf4e-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="6bf4e-107">· Get-User <email address></span></span>

<span data-ttu-id="6bf4e-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="6bf4e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="6bf4e-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="6bf4e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="6bf4e-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="6bf4e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="6bf4e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="6bf4e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="6bf4e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="6bf4e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="6bf4e-113">若要解決此問題，請删除具有相同電子郵件識別的多個物件，並確保存在一個具有特定電子郵件識別的物件，並且其收件者類型為 UserMailbox。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="6bf4e-114">**商務和消費者信箱使用同一地址**</span><span class="sxs-lookup"><span data-stu-id="6bf4e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="6bf4e-115">另一個原因是，商務和消費者信箱使用相同的位址。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="6bf4e-116">在此情況下，使用者必須變更其主要消費者別名，直到咖啡廳支援此案例。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="6bf4e-117">這是永久性錯誤，沒有干預就不能消失。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="6bf4e-118">如需詳細資訊，請參閱[變更您 Microsoft 帳戶的電子郵件地址或電話號碼](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)。</span><span class="sxs-lookup"><span data-stu-id="6bf4e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>