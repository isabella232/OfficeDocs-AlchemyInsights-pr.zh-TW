---
title: 修正 Microsoft 365 應用程式無法找到與 office 授權相關聯的郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747686"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="3c46e-102">修正 Microsoft 365 應用程式「找不到相關聯的 office 授權」訊息</span><span class="sxs-lookup"><span data-stu-id="3c46e-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="3c46e-103">如果您收到這封郵件，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="3c46e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3c46e-104">檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖對 Microsoft 365 應用程式的網際網路存取。</span><span class="sxs-lookup"><span data-stu-id="3c46e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3c46e-105">請參閱 [Microsoft 365 URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。</span><span class="sxs-lookup"><span data-stu-id="3c46e-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="3c46e-106">移除並 [重新指派受影響使用者的 Office 授權](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 。</span><span class="sxs-lookup"><span data-stu-id="3c46e-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="3c46e-107">開啟 Office 應用程式， [並登出](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 任何現有的使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="3c46e-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="3c46e-108">移至 Windows 設定 >**帳戶**  >  **電子郵件 & 帳戶**，並移除所有的工作帳戶（受影響的帳戶除外）。</span><span class="sxs-lookup"><span data-stu-id="3c46e-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="3c46e-109">移至 Windows 設定 >**帳戶**  >  **存取工作或學校**，並中斷所有工作帳戶（受影響的帳戶除外）的連線。</span><span class="sxs-lookup"><span data-stu-id="3c46e-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="3c46e-110">重設 Office 啟用狀態。</span><span class="sxs-lookup"><span data-stu-id="3c46e-110">Reset the Office activation state.</span></span> <span data-ttu-id="3c46e-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3c46e-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="3c46e-112">使用受影響的使用者帳戶登[入](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="3c46e-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="3c46e-113">如需其他疑難排解解決方案，請參閱 [Office 中的未經許可產品和啟用錯誤](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="3c46e-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>