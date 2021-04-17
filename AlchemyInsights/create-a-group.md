---
title: 建立群組
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816339"
---
# <a name="create-a-group"></a><span data-ttu-id="c06aa-102">建立群組</span><span class="sxs-lookup"><span data-stu-id="c06aa-102">Create a group</span></span>

<span data-ttu-id="c06aa-103">本主題說明群組的建立。</span><span class="sxs-lookup"><span data-stu-id="c06aa-103">This topic describes group creation.</span></span>

<span data-ttu-id="c06aa-104">**建立群組的許可權**</span><span class="sxs-lookup"><span data-stu-id="c06aa-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="c06aa-105">確定您有權建立新的群組。</span><span class="sxs-lookup"><span data-stu-id="c06aa-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="c06aa-106">全域系統管理員可以在 Azure 入口網站或存取面板中停用群組建立。</span><span class="sxs-lookup"><span data-stu-id="c06aa-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="c06aa-107">您可能需要系統管理員才能建立新群組，或提供您適當權限。</span><span class="sxs-lookup"><span data-stu-id="c06aa-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="c06aa-108">**管理群組建立權限**</span><span class="sxs-lookup"><span data-stu-id="c06aa-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="c06aa-109">全域管理員可以在 azure 入口網站或 Access 面板中，透過選擇「使用者可以在 azure 入口網站中建立安全性群組」或「使用者 **可以在 azure** 入口網站中建立 Office 365 群組」  >  **)  (** 選項，管理群組建立許可權 (以) 或 Office 365 群組的安全性相關的原因。</span><span class="sxs-lookup"><span data-stu-id="c06aa-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="c06aa-110">您也可以限制群組建立，以選取一組使用者，如果您擁有 Azure Active Directory P1 優質授權。</span><span class="sxs-lookup"><span data-stu-id="c06aa-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="c06aa-111">**停用新 Office 365 群組成員的歡迎使用通知**</span><span class="sxs-lookup"><span data-stu-id="c06aa-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="c06aa-112">在 Powershell 中將 **UnifiedGroupWelcomeMessageEnabled** 設定為 False，即可停用傳送給新增至 Office 365 群組之使用者的歡迎使用通知。</span><span class="sxs-lookup"><span data-stu-id="c06aa-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="c06aa-113">在[這裡](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)深入了解此設定。</span><span class="sxs-lookup"><span data-stu-id="c06aa-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

