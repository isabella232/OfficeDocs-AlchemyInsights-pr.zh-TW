---
title: 封鎖使用者建立的電子郵件簽名
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232695"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="cb86c-102">封鎖使用者建立的電子郵件簽名</span><span class="sxs-lookup"><span data-stu-id="cb86c-102">Block user-made email signatures</span></span>

<span data-ttu-id="cb86c-103">下列解決方案只適用于在 web 上的 Outlook 中建立的電子郵件簽名。</span><span class="sxs-lookup"><span data-stu-id="cb86c-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="cb86c-104">如果您有內部部署 Exchange 伺服器，您就只能封鎖 Outlook 應用程式中的簽章。</span><span class="sxs-lookup"><span data-stu-id="cb86c-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="cb86c-105">在系統管理中心中，選擇 [系統 **管理中心**] [  >  **Exchange**]。</span><span class="sxs-lookup"><span data-stu-id="cb86c-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="cb86c-106">按一下 [**許可權**] [  >  **Outlook Web App 原則**]。</span><span class="sxs-lookup"><span data-stu-id="cb86c-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="cb86c-107">選取原則，然後按一下鉛筆圖示進行編輯。</span><span class="sxs-lookup"><span data-stu-id="cb86c-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="cb86c-108">按一下 [其他 **功能**  >  **選項**]。</span><span class="sxs-lookup"><span data-stu-id="cb86c-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="cb86c-109">在 [ **使用者經驗**] 底下，清除 [ **電子郵件簽名** ] 核取方塊，然後按一下 [ **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="cb86c-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="cb86c-110">**重要：** 如果在清除此核取方塊之前新增了簽名，使用者仍可使用它。</span><span class="sxs-lookup"><span data-stu-id="cb86c-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="cb86c-111">要求他們移除。</span><span class="sxs-lookup"><span data-stu-id="cb86c-111">Ask them to remove it.</span></span>
