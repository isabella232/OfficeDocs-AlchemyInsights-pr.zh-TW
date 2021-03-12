---
title: 密碼原則
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718185"
---
# <a name="password-policies"></a><span data-ttu-id="6d533-102">密碼原則</span><span class="sxs-lookup"><span data-stu-id="6d533-102">Password policies</span></span>

<span data-ttu-id="6d533-103">**我在使用使用者的密碼原則時發生問題**</span><span class="sxs-lookup"><span data-stu-id="6d533-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="6d533-104">使用者的密碼原則取決於使用者是否僅限雲端或內部部署。</span><span class="sxs-lookup"><span data-stu-id="6d533-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="6d533-105">僅限雲端使用者必須選擇符合本文中需求的密碼： [僅適用于雲端使用者帳戶的密碼原則](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="6d533-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="6d533-106">內部部署使用者必須選擇符合內部部署需求的密碼。</span><span class="sxs-lookup"><span data-stu-id="6d533-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="6d533-107">如果內部部署使用者無法設定其密碼，請檢查您的內部部署需求。</span><span class="sxs-lookup"><span data-stu-id="6d533-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="6d533-108">**我不知道如何設定或檢查密碼到期原則**</span><span class="sxs-lookup"><span data-stu-id="6d533-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="6d533-109">您可以使用 PowerShell 來設定及檢查您租使用者中的雲端使用者到期原則。</span><span class="sxs-lookup"><span data-stu-id="6d533-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="6d533-110">遵循本文中的指示： [使用 PowerShell 設定或檢查密碼原則](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="6d533-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="6d533-111">內部部署使用者的密碼到期原則是在您的內部部署 AD 中設定。</span><span class="sxs-lookup"><span data-stu-id="6d533-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="6d533-112">**其他有用的連結：**</span><span class="sxs-lookup"><span data-stu-id="6d533-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="6d533-113">密碼重設入門</span><span class="sxs-lookup"><span data-stu-id="6d533-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="6d533-114">疑難排解管理員初始化的密碼重設</span><span class="sxs-lookup"><span data-stu-id="6d533-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
