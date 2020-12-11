---
title: 使用 Microsoft Intune 管理 iOS 和 Android 的 Microsoft Edge 中的 web access
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617244"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="c4c6e-102">使用 Microsoft Intune 管理 iOS 和 Android 的 Microsoft Edge 中的 web access</span><span class="sxs-lookup"><span data-stu-id="c4c6e-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="c4c6e-103">用於 iOS 和 Android 的 Microsoft Edge 可讓使用者從多個完全不同的設定檔流覽網頁。</span><span class="sxs-lookup"><span data-stu-id="c4c6e-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="c4c6e-104">當您訂閱 Enterprise 可移動性 + 安全套件（包括 Microsoft Intune 和 Azure Active Directory Premium 功能，例如條件式存取）時，Microsoft 365 資料的最大保護功能會變成可用。</span><span class="sxs-lookup"><span data-stu-id="c4c6e-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="c4c6e-105">在最低限度下，您會想要部署 (1) 的條件式存取原則，讓使用者從行動裝置連線至 Microsoft Edge 以取得 iOS 和 Android，而且 (2) 會執行 Microsoft Intune 應用程式保護原則，提供受保護的流覽體驗。</span><span class="sxs-lookup"><span data-stu-id="c4c6e-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="c4c6e-106">若要瞭解您可以如何使用條件式存取和原則，請參閱：</span><span class="sxs-lookup"><span data-stu-id="c4c6e-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="c4c6e-107">套用 Azure Active Directory 條件式存取原則</span><span class="sxs-lookup"><span data-stu-id="c4c6e-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="c4c6e-108">建立 Microsoft Intune 應用程式保護原則</span><span class="sxs-lookup"><span data-stu-id="c4c6e-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="c4c6e-109">在原則保護的瀏覽器中，針對 Azure Active Directory 連線的 web 應用程式使用單一登入</span><span class="sxs-lookup"><span data-stu-id="c4c6e-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="c4c6e-110">使用應用程式設定來管理流覽體驗</span><span class="sxs-lookup"><span data-stu-id="c4c6e-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="c4c6e-111">僅允許使用工作和學校帳戶</span><span class="sxs-lookup"><span data-stu-id="c4c6e-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="c4c6e-112">部署一般應用程式佈建原則</span><span class="sxs-lookup"><span data-stu-id="c4c6e-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="c4c6e-113">部署資料保護的應用程式佈建原則</span><span class="sxs-lookup"><span data-stu-id="c4c6e-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="c4c6e-114">使用 Microsoft 端點管理員部署應用程式佈建原則</span><span class="sxs-lookup"><span data-stu-id="c4c6e-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="c4c6e-115">若要瞭解如何存取受管理的應用程式記錄檔，請參閱 [使用 Microsoft Edge for iOS 和 Android 存取受管理的應用程式記錄](https://go.microsoft.com/fwlink/?linkid=2132578)檔。</span><span class="sxs-lookup"><span data-stu-id="c4c6e-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
