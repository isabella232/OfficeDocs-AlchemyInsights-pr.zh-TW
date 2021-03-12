---
title: 啟用 DKIM 的自訂網域
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735992"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="59287-102">啟用 DKIM 的自訂網域</span><span class="sxs-lookup"><span data-stu-id="59287-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="59287-103">在您為自訂網域建立 CNAME 記錄之後，您必須啟用網域。</span><span class="sxs-lookup"><span data-stu-id="59287-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="59287-104">若要啟用網域，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="59287-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="59287-105">流覽至 [Exchange 系統管理中心](https://outlook.office365.com/ecp/)。</span><span class="sxs-lookup"><span data-stu-id="59287-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="59287-106">在左窗格中，選取 [ **保護 > dkim**]。</span><span class="sxs-lookup"><span data-stu-id="59287-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="59287-107">選取 [網域]，然後在 [ **使用 DKIM 簽章簽署此網域的郵件**] 底下，按一下 [ **啟用**]。</span><span class="sxs-lookup"><span data-stu-id="59287-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="59287-108">針對每個網域重複此步驟。</span><span class="sxs-lookup"><span data-stu-id="59287-108">Repeat this step for each domain.</span></span>

