---
title: 關於 Yammer 中的身分識別
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664161"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="fe2a4-102">關於 Yammer 中的身分識別</span><span class="sxs-lookup"><span data-stu-id="fe2a4-102">About identity in Yammer</span></span>

<span data-ttu-id="fe2a4-103">建議所有網路採取以下步驟，以避免身分識別相關問題:</span><span class="sxs-lookup"><span data-stu-id="fe2a4-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="fe2a4-104">在 Azure AD 中為使用者提供 Microsoft 365 帳戶後，強制執行 Office 365 身分識別，以確保所有使用者都使用自己的主要 Microsoft 365 帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="fe2a4-105">如需詳細資訊，請參閱 [針對 Yammer 使用者強制執行 Office 365 身分識別](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="fe2a4-106">合併多個 Yammer 網路。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="fe2a4-107">舊版 Yammer 設定允許多個 Yammer 網路連線到一個租使用者。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="fe2a4-108">如需詳細資訊，請參閱[網路移轉 - 合併多個 Yammer 網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="fe2a4-109">您也可以選擇強制執行 Yammer 授權，以封鎖 Yammer 中沒有授權的使用者。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="fe2a4-110">如需詳細諮詢，請參閱 [在 Office 365 中管理 Yammer 使用者授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="fe2a4-111">最後，稽核之前的 Yammer 網路使用者清單，並暫停舊版使用者。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="fe2a4-112">建議您暫停（停用）使用者，而不是刪除使用者，因為刪除操作不可逆。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="fe2a4-113">如需詳細資訊，請參閱[稽核已連結至 Office 365 網路的 Yammer 使用者](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365)，並[移除使用者](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="fe2a4-114">透過使用下列步驟來設定 Yammer，您也可以準備將 您的 Yammer 網路設定為適用於 Microsoft 365 的原生模式。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="fe2a4-115">如需詳細資訊，請參閱 [針對適用於 Microsoft 365 的原生模式設定您的 Yammer 網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)。</span><span class="sxs-lookup"><span data-stu-id="fe2a4-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>