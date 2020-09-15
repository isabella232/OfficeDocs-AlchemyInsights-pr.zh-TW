---
title: 在 Exchange Online 中建立及共用公用資料夾行事曆
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712641"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="8b8ad-102">在 Exchange Online 中建立及共用公用資料夾行事曆</span><span class="sxs-lookup"><span data-stu-id="8b8ad-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="8b8ad-103">您只能從 Outlook 桌面用戶端建立公用資料夾中的行事曆。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="8b8ad-104">使用下列步驟設定公用資料夾行事曆：</span><span class="sxs-lookup"><span data-stu-id="8b8ad-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="8b8ad-105">確定 Exchange Online 中有部署公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="8b8ad-106">如需詳細資訊，請參閱[建立公用資料夾信箱](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="8b8ad-107">請確定您已獲指派建立公用資料夾所必要的存取權限。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="8b8ad-108">如需詳細資訊，請參閱 [Exchange Server 的公用資料夾權限](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="8b8ad-109">登入 Outlook 桌面用戶端，並確保您可以存取公用資料夾部署。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="8b8ad-110">如果您無法使用 Outlook 桌面用戶端存取公用資料夾，請參閱 [Exchange Online 使用者無法使用 Outlook 或 OWA 連線到公用資料夾](https://aka.ms/pfcte)。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="8b8ad-111">建立新的公用資料夾行事曆類型。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="8b8ad-112">預設會將公用資料夾共用給其他所有使用者。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="8b8ad-113">公用資料夾擁有者可以從 Outlook 桌面用戶端變更權限。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="8b8ad-114">如需詳細資訊，請參閱 [Exchange Server 的公用資料夾權限](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="8b8ad-115">**附註**：公用資料夾行事曆是專為在組織內部使用而設計，無法在網際網路上發佈。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="8b8ad-116">如果您想要將行事曆發佈到網際網路，請使用共用信箱。</span><span class="sxs-lookup"><span data-stu-id="8b8ad-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>