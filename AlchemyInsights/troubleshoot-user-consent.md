---
title: 疑難排解使用者的同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897702"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="df582-102">疑難排解使用者的同意</span><span class="sxs-lookup"><span data-stu-id="df582-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="df582-103">您可以設定使用者同意透過 Azure 入口網站或 PowerShell 的應用程式。</span><span class="sxs-lookup"><span data-stu-id="df582-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="df582-104">如需詳細資訊，請參閱 [使用者同意設定](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 。</span><span class="sxs-lookup"><span data-stu-id="df582-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="df582-105">管理員也可以使用 [Microsoft GRAPH API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) ，以代表單一使用者授與委派許可權。</span><span class="sxs-lookup"><span data-stu-id="df582-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="df582-106">如需詳細資訊，請參閱 [代表使用者取得存取權](https://docs.microsoft.com/graph/auth-v2-user)。</span><span class="sxs-lookup"><span data-stu-id="df582-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="df582-107">[使用者同意錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)：本文討論在同意應用程式期間可能發生的錯誤。</span><span class="sxs-lookup"><span data-stu-id="df582-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="df582-108">如果您正在疑難排解未包含任何錯誤訊息的意外同意提示，請參閱 [AZURE AD 的驗證案例](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。</span><span class="sxs-lookup"><span data-stu-id="df582-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>