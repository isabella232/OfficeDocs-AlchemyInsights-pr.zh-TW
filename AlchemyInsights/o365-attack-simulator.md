---
title: Microsoft 365 中的2681攻擊模擬器
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713457"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="799ff-102">Microsoft 365 中的攻擊模擬器</span><span class="sxs-lookup"><span data-stu-id="799ff-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="799ff-103">您是否遺漏攻擊模擬器？</span><span class="sxs-lookup"><span data-stu-id="799ff-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="799ff-104">攻擊模擬器需要**Office 365 高級威脅防護方案2（ATP 方案2）** 或**Office 365 企業版 E5**。</span><span class="sxs-lookup"><span data-stu-id="799ff-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="799ff-105">「Office 365 高級威脅防護方案1（ATP 方案1）」、Office 365 企業版 E3 或任何 Microsoft 365 Apps for business 訂閱中**不**包含攻擊模擬器。</span><span class="sxs-lookup"><span data-stu-id="799ff-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="799ff-106">您用來啟動模擬攻擊的帳戶需要全域系統管理員或安全性管理員許可權，以及多重要素驗證（MFA）。</span><span class="sxs-lookup"><span data-stu-id="799ff-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="799ff-107">如需有關攻擊模擬程式需求的詳細資訊，請參閱[本主題](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)。</span><span class="sxs-lookup"><span data-stu-id="799ff-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="799ff-108">關於**強力強制密碼**攻擊模擬的重要事項：</span><span class="sxs-lookup"><span data-stu-id="799ff-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="799ff-109">如果目標帳戶已啟用 MFA，且密碼猜測正確，該帳戶將不會顯示為 [已遭破壞] （第二個驗證因素將不完整）。</span><span class="sxs-lookup"><span data-stu-id="799ff-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="799ff-110">密碼檔不可超過 10 MB。</span><span class="sxs-lookup"><span data-stu-id="799ff-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="799ff-111">每行使用一個密碼，並在清單中的最後一個密碼之後加入一條空白行（回車）。</span><span class="sxs-lookup"><span data-stu-id="799ff-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="799ff-112">**Spear 網路釣魚**附加模擬所需注意的重要事項：</span><span class="sxs-lookup"><span data-stu-id="799ff-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="799ff-113">根據設計，您無法為**網路釣魚登入伺服器 URL**提供自訂值。</span><span class="sxs-lookup"><span data-stu-id="799ff-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="799ff-114">如果收件者使用「[啟用報告訊息增益集](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)」，將郵件報告為網路釣魚，您可能不會收到郵件的警示（因為這是模擬型攻擊）。</span><span class="sxs-lookup"><span data-stu-id="799ff-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="799ff-115">報告：模擬的攻擊完成後，您可以按一下 [**攻擊詳細資料**] 以查看報告。</span><span class="sxs-lookup"><span data-stu-id="799ff-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="799ff-116">如需攻擊模擬器的詳細指示和新功能，請參閱[Microsoft 365 中的攻擊模擬器](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。</span><span class="sxs-lookup"><span data-stu-id="799ff-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
