---
title: 新式 Azure 電子郵件發票開立
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820817"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="f6021-102">Azure 中的電子郵件發票開立</span><span class="sxs-lookup"><span data-stu-id="f6021-102">Email invoicing in Azure</span></span>

<span data-ttu-id="f6021-103">您必須在帳單設定檔或其計費帳戶上具有擁有者或投稿人角色，才能更新其電子郵件發票喜好設定。</span><span class="sxs-lookup"><span data-stu-id="f6021-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="f6021-104">一旦您選擇加入，所有在賬單設定檔中具有擁有者、投稿人、讀取者和發票管理員角色的使用者都將透過電子郵件獲得其發票。</span><span class="sxs-lookup"><span data-stu-id="f6021-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="f6021-105">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="f6021-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f6021-106">搜尋 **[成本管理] + [計費]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="f6021-107">從左側選取 **[發票]**，然後選取頁面頂端的 **[電子郵件發票]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="f6021-108">如果您有多個賬單設定檔，請選取帳單設定檔，然後選取 **[選擇加入]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="f6021-109">選取 **[更新]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-109">Select **Update**.</span></span>
6. <span data-ttu-id="f6021-110">如果您有多個賬單設定檔，請選取帳單設定檔，然後選取 **[選擇加入]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="f6021-111">透過為其他人指派 MCA 或 MPA 賬單設定檔的發票管理員角色，可以為其他人提供檢視、下載和支付發票的存取權。</span><span class="sxs-lookup"><span data-stu-id="f6021-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="f6021-112">如果您選擇在電子郵件中取得發票，使用者也會收到電子郵件中的發票。</span><span class="sxs-lookup"><span data-stu-id="f6021-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="f6021-113">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="f6021-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f6021-114">搜尋 **[成本管理] + [計費]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="f6021-115">從左側選取 **[帳單設定檔]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="f6021-116">從 [賬單設定檔] 清單中，選取您要指派發票管理員角色的帳單設定檔。</span><span class="sxs-lookup"><span data-stu-id="f6021-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="f6021-117">從左側選取 **[存取控制] (IAM)** ，然後從頁面頂端選取 **[新增]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="f6021-118">在 [角色] 下拉式清單中，選取 **[發票管理員]**。</span><span class="sxs-lookup"><span data-stu-id="f6021-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="f6021-119">輸入要授與存取權的使用者電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="f6021-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="f6021-120">選取 **[儲存]** 以指派角色。</span><span class="sxs-lookup"><span data-stu-id="f6021-120">Select **Save** to assign the role.</span></span>
