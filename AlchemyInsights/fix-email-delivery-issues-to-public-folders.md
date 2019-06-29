---
title: 修正已啟用郵件功能之公用資料夾的電子郵件傳遞問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387696"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="e87f9-102">修正已啟用郵件功能之公用資料夾的電子郵件傳遞問題</span><span class="sxs-lookup"><span data-stu-id="e87f9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="e87f9-103">如果外部寄件者無法傳送郵件至擁有郵件功能的公用資料夾, 且寄件者收到錯誤:**無法找到 (550 5.4.1)**, 請確認公用資料夾的電子郵件網域設定為內部轉送網域, 而不是授權網域:</span><span class="sxs-lookup"><span data-stu-id="e87f9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="e87f9-104">開啟[Exchange 系統管理中心 (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="e87f9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="e87f9-105">移至 [**郵件流程** \> ] [**公認的網域**], 選取公認的網域, 然後按一下 [**編輯**]。</span><span class="sxs-lookup"><span data-stu-id="e87f9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="e87f9-106">在開啟的 [屬性] 頁面中, 如果將網欄位型別設定為 [**授權**], 請將值變更為 [**內部轉送**], 然後按一下 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="e87f9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="e87f9-107">如果外部寄件者收到錯誤, 表示**您沒有許可權 (550 5.7.13)**, 請在[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行下列命令, 以查看公用資料夾中匿名使用者的許可權:</span><span class="sxs-lookup"><span data-stu-id="e87f9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="e87f9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`例如, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`。</span><span class="sxs-lookup"><span data-stu-id="e87f9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="e87f9-109">若要允許外部使用者將電子郵件傳送至此公用資料夾, 請將 CreateItems 存取權限新增至匿名使用者。</span><span class="sxs-lookup"><span data-stu-id="e87f9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="e87f9-110">例如 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。</span><span class="sxs-lookup"><span data-stu-id="e87f9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
