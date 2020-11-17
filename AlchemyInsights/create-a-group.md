---
title: 建立群組
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086290"
---
# <a name="create-a-group"></a><span data-ttu-id="94f11-102">建立群組</span><span class="sxs-lookup"><span data-stu-id="94f11-102">Create a group</span></span>

<span data-ttu-id="94f11-103">本主題說明群組的建立。</span><span class="sxs-lookup"><span data-stu-id="94f11-103">This topic describes group creation.</span></span>

<span data-ttu-id="94f11-104">**建立群組的許可權**</span><span class="sxs-lookup"><span data-stu-id="94f11-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="94f11-105">確定您有權建立新的群組。</span><span class="sxs-lookup"><span data-stu-id="94f11-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="94f11-106">全域管理員可以停用 Azure 入口網站或存取面板中的群組建立。</span><span class="sxs-lookup"><span data-stu-id="94f11-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="94f11-107">您可能需要管理員為您建立新的群組，或為您提供適當的許可權。</span><span class="sxs-lookup"><span data-stu-id="94f11-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="94f11-108">**管理群組建立許可權**</span><span class="sxs-lookup"><span data-stu-id="94f11-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="94f11-109">全域管理員可以在 azure 入口網站或 Access 面板中，透過選擇「使用者可以在 azure 入口網站中建立安全性群組」或「使用者 **可以在 azure** 入口網站中建立 Office 365 群組」  >  **)  (** 選項，管理群組建立許可權 (以) 或 Office 365 群組的安全性相關的原因。</span><span class="sxs-lookup"><span data-stu-id="94f11-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="94f11-110">您也可以限制群組建立，以選取一組使用者，如果您擁有 Azure Active Directory P1 優質授權。</span><span class="sxs-lookup"><span data-stu-id="94f11-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="94f11-111">**停用新 Office 365 群組成員的歡迎使用通知**</span><span class="sxs-lookup"><span data-stu-id="94f11-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="94f11-112">在 Powershell 中將 **UnifiedGroupWelcomeMessageEnabled** 設定為 False，即可停用傳送給新增至 Office 365 群組之使用者的歡迎使用通知。</span><span class="sxs-lookup"><span data-stu-id="94f11-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="94f11-113">若要深入瞭解 [，請參閱此設定](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="94f11-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

