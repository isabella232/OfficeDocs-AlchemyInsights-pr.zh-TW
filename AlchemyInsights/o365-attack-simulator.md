---
title: Microsoft 365 中的2681攻擊模擬器
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545717"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="2f148-102">Microsoft 365 中的攻擊模擬器</span><span class="sxs-lookup"><span data-stu-id="2f148-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="2f148-103">您是否遺漏攻擊模擬器？</span><span class="sxs-lookup"><span data-stu-id="2f148-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="2f148-104">攻擊模擬 **程式需要 Microsoft Defender Office 365 方案 2** 或 **Office 365 企業版 E5**。</span><span class="sxs-lookup"><span data-stu-id="2f148-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="2f148-105">Microsoft Defender 中 **未** 包含攻擊模擬器，以 Office 365 方案1、Office 365 企業版 E3 或任何 Microsoft 365 Apps 商務版訂閱。</span><span class="sxs-lookup"><span data-stu-id="2f148-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="2f148-106">您用來啟動模擬攻擊的帳戶需要全域系統管理員或安全性管理員許可權，以及多重要素驗證 (MFA) 。</span><span class="sxs-lookup"><span data-stu-id="2f148-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="2f148-107">如需有關攻擊模擬程式需求的詳細資訊，請參閱 [本主題](/microsoft-365/security/office-365-security/attack-simulator)。</span><span class="sxs-lookup"><span data-stu-id="2f148-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="2f148-108">關於 **強力強制密碼** 攻擊模擬的重要事項：</span><span class="sxs-lookup"><span data-stu-id="2f148-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="2f148-109">如果目標帳戶已啟用 MFA，且密碼猜測正確，則此帳戶不會顯示 (第二個驗證因素) 不完整的帳戶。</span><span class="sxs-lookup"><span data-stu-id="2f148-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="2f148-110">密碼檔不可超過 10 MB。</span><span class="sxs-lookup"><span data-stu-id="2f148-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="2f148-111">每行使用一個密碼，並在清單中的最後一個密碼之後 (回車) 中包含一條空行。</span><span class="sxs-lookup"><span data-stu-id="2f148-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="2f148-112">**Spear 網路釣魚** 附加模擬所需注意的重要事項：</span><span class="sxs-lookup"><span data-stu-id="2f148-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="2f148-113">根據設計，您無法為 **網路釣魚登入伺服器 URL** 提供自訂值。</span><span class="sxs-lookup"><span data-stu-id="2f148-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="2f148-114">如果收件者使用「 [啟用報告訊息增益集](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 」，將郵件報告為網路釣魚，您可能不會收到郵件 (的提醒，因為這是模擬型攻擊) 。</span><span class="sxs-lookup"><span data-stu-id="2f148-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="2f148-115">報告：模擬的攻擊完成後，您可以按一下 [ **攻擊詳細資料** ] 以查看報告。</span><span class="sxs-lookup"><span data-stu-id="2f148-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="2f148-116">如需攻擊模擬器中的詳細指示和新功能，請參閱[Microsoft 365 中的攻擊模擬器](/microsoft-365/security/office-365-security/attack-simulator)。</span><span class="sxs-lookup"><span data-stu-id="2f148-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
