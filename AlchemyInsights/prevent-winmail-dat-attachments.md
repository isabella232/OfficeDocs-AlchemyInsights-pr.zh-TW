---
title: 2589協助防止來自組織之電子郵件的 Winmail.dat .dat 附件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693726"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="b07f7-102">協助防止來自組織的電子郵件中的 Winmail.dat 附件</span><span class="sxs-lookup"><span data-stu-id="b07f7-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="b07f7-103">以管理員身分，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="b07f7-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="b07f7-104">開啟 [Exchange 系統管理中心][](https://outlook.office365.com/ecp/)。</span><span class="sxs-lookup"><span data-stu-id="b07f7-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="b07f7-105">移至 [**郵件流程**]  >  **遠端網域**。</span><span class="sxs-lookup"><span data-stu-id="b07f7-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="b07f7-106">選取名為 **default**的預設遠端網域，然後按一下 [ **編輯**]。</span><span class="sxs-lookup"><span data-stu-id="b07f7-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="b07f7-107">在 [ **使用 rtf 格式** ] 區段中，選取 [ **從不**]。</span><span class="sxs-lookup"><span data-stu-id="b07f7-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="b07f7-108">如需詳細資訊，請參閱 [指定遠端網域的郵件格式](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)。</span><span class="sxs-lookup"><span data-stu-id="b07f7-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
