---
title: 無法啟用 Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 50939456df57920994e464db20e5da54f45f197a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744617"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="528c9-102">無法啟用 Office</span><span class="sxs-lookup"><span data-stu-id="528c9-102">Unable to activate Office</span></span>

- <span data-ttu-id="528c9-103">檢查您的訂閱狀態是否已過期。</span><span class="sxs-lookup"><span data-stu-id="528c9-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="528c9-104">確認您擁有允許用戶端授權的訂閱 (例如 Office 365 商務版或商務進階版)，並[確保該使用者已獲派授權](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users)。</span><span class="sxs-lookup"><span data-stu-id="528c9-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="528c9-105">請確認使用者使用所指派授權的相同帳戶登入 Office。</span><span class="sxs-lookup"><span data-stu-id="528c9-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="528c9-106">查看 [Office 365 服務健康情況頁面](https://docs.microsoft.com/office365/enterprise/view-service-health)，以查看服務是否有任何已知問題。</span><span class="sxs-lookup"><span data-stu-id="528c9-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="528c9-107">檢查您的防火牆、防毒軟體和 Proxy 設定，確認未封鎖 Microsoft 365 應用程式存取網際網路。</span><span class="sxs-lookup"><span data-stu-id="528c9-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="528c9-108">若要深入了解，請參閱 [Office 365 URL 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 和 IP 位址範圍") (英文)。</span><span class="sxs-lookup"><span data-stu-id="528c9-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="528c9-109">請使用下列疑難排解動作：</span><span class="sxs-lookup"><span data-stu-id="528c9-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="528c9-110">開啟 Office App，並 [[登出]](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何現有的使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="528c9-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="528c9-111">[[移除]](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 並 [[重新指派]](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office 授權，然後使用受影響的使用者帳戶 [[登入 Office]](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="528c9-111">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="528c9-112">執行 [[啟用疑難排解員]](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="528c9-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="528c9-113">重設 Office 啟用狀態</span><span class="sxs-lookup"><span data-stu-id="528c9-113">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "重設 Office 啟用狀態")
- [<span data-ttu-id="528c9-114">執行 Office 線上修復</span><span class="sxs-lookup"><span data-stu-id="528c9-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="528c9-115">如需其他疑難排解解決方案，請參閱：</span><span class="sxs-lookup"><span data-stu-id="528c9-115">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="528c9-116">Office 中的「未授權產品」及啟用錯誤</span><span class="sxs-lookup"><span data-stu-id="528c9-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- <span data-ttu-id="528c9-117">[啟用 Office 時，「很抱歉，我們無法連線至您的帳戶。請稍後再試一次」的錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365) (英文)</span><span class="sxs-lookup"><span data-stu-id="528c9-117">["Sorry, we can't connect to your account. Please try again later" error when you activate Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span></span>