---
title: 防禦退信攻擊
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897706"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="5f481-102">防禦退信攻擊</span><span class="sxs-lookup"><span data-stu-id="5f481-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="5f481-103">退信攻擊是您對於未寄送過的郵件所收到的未傳遞報告 (也稱為 NDR 或退回的郵件)。</span><span class="sxs-lookup"><span data-stu-id="5f481-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="5f481-104">濫發垃圾郵件者偽造 (詐騙) 其郵件的 **寄件者：** 地址，他們通常會使用實際的電子郵件地址來增加郵件的可信度。</span><span class="sxs-lookup"><span data-stu-id="5f481-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="5f481-105">因此，當濫發垃圾郵件者將郵件傳送給不存在的收件者時，目的地電子郵件伺服器基本上會遭到誘拐而透過 NDR 將無法傳遞的郵件退回給 **寄件者：** 地址中的偽造寄件者。</span><span class="sxs-lookup"><span data-stu-id="5f481-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="5f481-106">其他資訊可以在 [EOP 中的退信攻擊](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)中找到。</span><span class="sxs-lookup"><span data-stu-id="5f481-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="5f481-107">**啟用退信攻擊保護**</span><span class="sxs-lookup"><span data-stu-id="5f481-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="5f481-108">若要啟用退信攻擊保護，請遵循下列路徑。</span><span class="sxs-lookup"><span data-stu-id="5f481-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="5f481-109">**protection.office.com > 威脅管理 > 原則 > 反垃圾郵件 > 選取垃圾郵件篩選原則並編輯原則 > 垃圾郵件屬性 > 標示為垃圾郵件 > NDR 退信攻擊 > 設為 [開啟]**</span><span class="sxs-lookup"><span data-stu-id="5f481-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="5f481-110">如果您認為帳戶已遭到入侵，請參閱下列內容：</span><span class="sxs-lookup"><span data-stu-id="5f481-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="5f481-111">回應遭入侵的電子郵件帳戶</span><span class="sxs-lookup"><span data-stu-id="5f481-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- <span data-ttu-id="5f481-112">[從 Office 365 中的 [受限使用者] 入口網站移除封鎖的使用者](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)</span><span class="sxs-lookup"><span data-stu-id="5f481-112">[Removing blocked users from the Restricted Users portal in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)</span></span>



