---
title: 管理同步處理的使用者
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380496"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="91806-102">無法設定主要電子郵件地址或變更使用者屬性</span><span class="sxs-lookup"><span data-stu-id="91806-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="91806-103">如果您的環境已啟用目錄同步處理, 則無法使用系統管理中心來變更某些使用者或物件屬性。</span><span class="sxs-lookup"><span data-stu-id="91806-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="91806-104">若要完整管理已同步處理的使用者及其所有屬性, 請使用您的本機 active directory 使用者和群組管理主控台 (adsiedit)。</span><span class="sxs-lookup"><span data-stu-id="91806-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="91806-105">或者, 您也可以使用 powershell 變更同步處理使用者的個別使用者或屬性, 如下列常見範例所示:</span><span class="sxs-lookup"><span data-stu-id="91806-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="91806-106">Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="91806-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="91806-107">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-部門 "HR"</span><span class="sxs-lookup"><span data-stu-id="91806-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="91806-108">Remove-Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="91806-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>