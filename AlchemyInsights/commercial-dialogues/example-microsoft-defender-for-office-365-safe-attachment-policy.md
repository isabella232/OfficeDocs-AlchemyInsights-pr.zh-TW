---
title: Microsoft Defender for Office 365 安全附件原則範例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735991"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="d5d8e-102">Microsoft Defender for Office 365 安全附件原則範例</span><span class="sxs-lookup"><span data-stu-id="d5d8e-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="d5d8e-103">這些設定可讓未設定 *延遲* 的原則立即傳遞郵件，然後在掃描後將附件：</span><span class="sxs-lookup"><span data-stu-id="d5d8e-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="d5d8e-104">**名稱**：無延遲</span><span class="sxs-lookup"><span data-stu-id="d5d8e-104">**Name**: No delays</span></span>
- <span data-ttu-id="d5d8e-105">**描述**：在掃描之後立即傳遞郵件並將附件。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="d5d8e-106">**回應**：選取 **動態傳遞** 選項。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="d5d8e-107">如需詳細資訊，請參閱 [在安全附件原則中的動態傳遞](https://go.microsoft.com/fwlink/?linkid=2092328)。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="d5d8e-108">重新 **導向附件** 區段：選取可 **啟用重新導向** 的選項，然後輸入您的 Microsoft 365 全域系統管理員、安全性管理員或將調查惡意附件的安全性分析員的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="d5d8e-109">**適用** 于區段：選取 **[收件者網域是**]，然後選取您的網域。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="d5d8e-110">選取 [ **新增**]，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="d5d8e-111">完成後，請選取 [ **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="d5d8e-112">若要深入瞭解，請參閱 [Microsoft Defender For Office 365 中的安全附件](https://go.microsoft.com/fwlink/?linkid=2092213)。</span><span class="sxs-lookup"><span data-stu-id="d5d8e-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
