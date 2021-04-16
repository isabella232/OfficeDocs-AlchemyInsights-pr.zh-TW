---
title: 設定電子郵件轉寄
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
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787128"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="a648f-102">檢查信箱的電子郵件轉送設定</span><span class="sxs-lookup"><span data-stu-id="a648f-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="a648f-103">首先，必須啟用租使用者層級的電子郵件轉接。</span><span class="sxs-lookup"><span data-stu-id="a648f-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="a648f-104">如果您已在信箱上設定電子郵件轉寄功能，但沒有運作 (您會收到錯誤「 **550 5.7.520 存取權遭到拒絕，您的組織不允許外部轉送** 」) 請參閱 [在 Microsoft 365 中控制自動外部電子郵件](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)轉寄。</span><span class="sxs-lookup"><span data-stu-id="a648f-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="a648f-105">很容易驗證信箱上的電子郵件轉送設定！</span><span class="sxs-lookup"><span data-stu-id="a648f-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="a648f-106">請遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="a648f-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="a648f-107">如果這是使用者信箱，請移至 [ **使用者**] [作用中的 \> **使用者** ]，然後選取您要轉寄其信箱的使用者。</span><span class="sxs-lookup"><span data-stu-id="a648f-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="a648f-108">在 [ **郵件** ] 索引標籤上，選取 [ **管理電子郵件轉發**]。</span><span class="sxs-lookup"><span data-stu-id="a648f-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="a648f-109">如果這是共用信箱，請移至 [**群組**] [共用信箱]， \> 然後選取您要轉送的共用信箱。</span><span class="sxs-lookup"><span data-stu-id="a648f-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="a648f-110">選取 [電子郵件轉發] 的 [ **編輯** ]。</span><span class="sxs-lookup"><span data-stu-id="a648f-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="a648f-111">如需詳細資訊，請參閱 [在 Microsoft 365 中設定電子郵件轉接](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。</span><span class="sxs-lookup"><span data-stu-id="a648f-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="a648f-112">若要將指示傳送給您的使用者，以便他們在自己的信箱上設定電子郵件轉寄功能，請將 [365 電子郵件轉寄至其他電子郵件帳戶](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)。</span><span class="sxs-lookup"><span data-stu-id="a648f-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="a648f-113">請注意，您只能轉寄一個電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="a648f-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="a648f-114">如果您需要設定一組人員的轉接，請在 [ **群組**) ] 底下建立通訊群組清單 (，將您的使用者新增至該群組，然後設定轉寄給該群組。</span><span class="sxs-lookup"><span data-stu-id="a648f-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="a648f-115">您是否有員工離開？</span><span class="sxs-lookup"><span data-stu-id="a648f-115">Do you have an employee leaving?</span></span> <span data-ttu-id="a648f-116">請參閱 [移除 Microsoft 365 中的離職員工](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) 以取得建議的步驟。</span><span class="sxs-lookup"><span data-stu-id="a648f-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>