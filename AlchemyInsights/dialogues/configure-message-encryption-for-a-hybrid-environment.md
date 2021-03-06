---
title: 為混合式環境設定郵件加密
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509665"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="fe8db-102">為混合式環境設定郵件加密</span><span class="sxs-lookup"><span data-stu-id="fe8db-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="fe8db-103">在混合式 Exchange 環境中，只有在透過 Exchange Online 路由傳送電子郵件時，內部部署使用者才能使用 Office 郵件加密傳送加密的電子郵件 (OME) 。</span><span class="sxs-lookup"><span data-stu-id="fe8db-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="fe8db-104">若要使用 OME 加密電子郵件，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="fe8db-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="fe8db-105">使用混合式設定 [嚮導](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) 設定混合式環境。</span><span class="sxs-lookup"><span data-stu-id="fe8db-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="fe8db-106">不需要特殊的步驟來設定加密。</span><span class="sxs-lookup"><span data-stu-id="fe8db-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="fe8db-107">如您平常那樣，[為加密設定郵件流程規則](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。</span><span class="sxs-lookup"><span data-stu-id="fe8db-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


