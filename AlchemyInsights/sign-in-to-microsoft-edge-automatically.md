---
title: 自動登入 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398720"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="6ac46-102">自動登入 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6ac46-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="6ac46-103">Microsoft Edge 會依照使用者裝置的設定方式，使用 OS 預設帳戶自動登入使用者。</span><span class="sxs-lookup"><span data-stu-id="6ac46-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="6ac46-104">每種類型的設備設定及其相依使用者登入處理常式的情形如下所述：</span><span class="sxs-lookup"><span data-stu-id="6ac46-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="6ac46-105">**裝置為混合式/AAD-J**：在 windows 10、下層 windows 和對應的伺服器版本上都可以使用此選項。</span><span class="sxs-lookup"><span data-stu-id="6ac46-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="6ac46-106">使用者會以其 Azure Active Directory (AD) 帳戶自動登入。</span><span class="sxs-lookup"><span data-stu-id="6ac46-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="6ac46-107">**裝置已加入網域**：您可以在 windows 10、下層 Windows 和對應的伺服器版本上使用此選項。</span><span class="sxs-lookup"><span data-stu-id="6ac46-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="6ac46-108">根據預設，具有網域帳戶的使用者不會自動登入;若要啟用自動登入，請使用 **ConfigureOnPremisesAccountAutoSignIn** 原則。</span><span class="sxs-lookup"><span data-stu-id="6ac46-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="6ac46-109">若要為使用 Azure AD 帳戶的使用者啟用自動登入，請考慮混合式加入其裝置。</span><span class="sxs-lookup"><span data-stu-id="6ac46-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="6ac46-110">**作業系統的預設帳戶為 Microsoft 帳戶**：在 WINDOWS 10 RS3 上可以使用此選項 (版本1709，組建 10.0.16299) 和更新版本。</span><span class="sxs-lookup"><span data-stu-id="6ac46-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="6ac46-111">在企業裝置上不可能發生此案例。</span><span class="sxs-lookup"><span data-stu-id="6ac46-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="6ac46-112">不過，如果 OS 預設帳戶是 Microsoft 帳戶，則 Microsoft Edge 會以 Microsoft 帳戶自動登入使用者。</span><span class="sxs-lookup"><span data-stu-id="6ac46-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
