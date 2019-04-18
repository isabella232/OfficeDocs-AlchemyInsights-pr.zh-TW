---
title: 擁有郵件功能的公用資料夾修正電子郵件傳遞問題
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910581"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="39a32-102">擁有郵件功能的公用資料夾修正電子郵件傳遞問題</span><span class="sxs-lookup"><span data-stu-id="39a32-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="39a32-103">如果外部寄件者無法傳送郵件至擁有郵件功能公用資料夾，並寄件者會收到錯誤：**找不到 (550 5.4.1)**，確認電子郵件網域的公用資料夾已設定為內部轉送網域，而不是授權網域：</span><span class="sxs-lookup"><span data-stu-id="39a32-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="39a32-104">開啟[Exchange 系統管理中心 (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="39a32-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="39a32-105">前往 [**郵件流程** \> **公認的網域**] 中，選取公認的網域，然後按一下 [**編輯**。</span><span class="sxs-lookup"><span data-stu-id="39a32-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="39a32-106">內容中的頁面，會隨即開啟，如果網域類型設為 [**授權**將值變更為**內部轉送**，然後按一下 [**儲存**。</span><span class="sxs-lookup"><span data-stu-id="39a32-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="39a32-107">如果外部寄件者會收到錯誤，**您沒有權限 (550 5.7.13)**，請查看在公用資料夾的匿名使用者的權限的[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="39a32-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="39a32-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`例如， `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`。</span><span class="sxs-lookup"><span data-stu-id="39a32-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="39a32-109">若要允許外部使用者能夠傳送電子郵件給此公用資料夾，請新增 CreateItems 存取權限給使用者匿名。</span><span class="sxs-lookup"><span data-stu-id="39a32-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="39a32-110">例如 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。</span><span class="sxs-lookup"><span data-stu-id="39a32-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
