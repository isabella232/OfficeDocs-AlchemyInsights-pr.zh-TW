---
title: 還原已刪除的表單
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
- "2547"
- "9000672"
ms.openlocfilehash: 6923c15c3cce90c98ae79181e978fba273ab6059
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662415"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="54fff-102">還原已刪除的表單</span><span class="sxs-lookup"><span data-stu-id="54fff-102">Restore a deleted form</span></span>

<span data-ttu-id="54fff-103">如果您已意外刪除 Microsoft Forms 中的表單，可以進行復原。</span><span class="sxs-lookup"><span data-stu-id="54fff-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="54fff-104">以刪除之表單的擁有者身分登入 Microsoft Forms。</span><span class="sxs-lookup"><span data-stu-id="54fff-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="54fff-105">選取 [ **回收站**]，然後選取您要復原的表單，然後選取 [ **還原**]。</span><span class="sxs-lookup"><span data-stu-id="54fff-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="54fff-106">還原後，選取 [ **回到我的表單] 頁面** 箭號。</span><span class="sxs-lookup"><span data-stu-id="54fff-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="54fff-107">只有表單的擁有者可以復原。</span><span class="sxs-lookup"><span data-stu-id="54fff-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="54fff-108">如果已停用或移除租使用者的帳戶，則只有全域系統管理員才能復原表單。</span><span class="sxs-lookup"><span data-stu-id="54fff-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="54fff-109">全域管理員必須具備表單會授權，才可執行還原。</span><span class="sxs-lookup"><span data-stu-id="54fff-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="54fff-110">只有在停用的使用者帳戶的30天內建立或從承租人中移除的表單，才能還原。</span><span class="sxs-lookup"><span data-stu-id="54fff-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="54fff-111">如果您是租使用者的全域系統管理員，而您想要從已刪除或已停用的帳戶復原表單，請將 [電子郵件地址] 取代為下列 URL: \*\* https://forms.office.com/Pages/delegatepage.aspx?originalowner= [電子郵件地址]\*\* 中已刪除或已停用之使用者的電子郵件地址。例如，如果您的電子郵件地址是 JOHNDOE@CONTOSO.COM，則 URL 會是： **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** 。</span><span class="sxs-lookup"><span data-stu-id="54fff-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="54fff-112">一旦您可以存取使用者的已刪除表單，請選取您要移動的表單，然後選取 [**其他表單動作**  >  **移動**]。</span><span class="sxs-lookup"><span data-stu-id="54fff-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="54fff-113">若要復原已刪除但已從組織中移除使用者的表單，全域管理員可以選擇復原使用者、重設使用者的密碼，然後在以該使用者的身分登入時，存取表單，將其移至另一個作用中的使用者。</span><span class="sxs-lookup"><span data-stu-id="54fff-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 