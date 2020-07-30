---
title: VPN 相關問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505189"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="7aacb-102">VPN 相關問題</span><span class="sxs-lookup"><span data-stu-id="7aacb-102">VPN related issues</span></span>

<span data-ttu-id="7aacb-103">MDM 用戶端的 VPN 連線成功實作，取決於可反映 VPN 基礎結構需求的正確部署設定檔。</span><span class="sxs-lookup"><span data-stu-id="7aacb-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="7aacb-104">有關正在調查的用戶端平台的適當設定，請參閱：</span><span class="sxs-lookup"><span data-stu-id="7aacb-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="7aacb-105">Windows 10 和 Windows 全息攝影版裝置設定使用 Intune 新增 VPN 連線</span><span class="sxs-lookup"><span data-stu-id="7aacb-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="7aacb-106">在 Microsoft Intune 中新增適用於 iOS 與 iPadOS 裝置的 VPN 設定</span><span class="sxs-lookup"><span data-stu-id="7aacb-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="7aacb-107">Android 裝置設定在 Intune 中設定 VPN </span><span class="sxs-lookup"><span data-stu-id="7aacb-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="7aacb-108">macOS 裝置新增 Microsoft Intune 中的 VPN 設定</span><span class="sxs-lookup"><span data-stu-id="7aacb-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="7aacb-109">如果您的 VPN 設定檔使用憑證型驗證，請確認已成功部署連結至 VPN 設定檔的根憑證和用戶端驗證憑證設定檔。</span><span class="sxs-lookup"><span data-stu-id="7aacb-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="7aacb-110">**常見問題**</span><span class="sxs-lookup"><span data-stu-id="7aacb-110">**Common Issues**</span></span>

<span data-ttu-id="7aacb-111">**我將 VPN 設定檔部署到裝置上。Intune 顯示它已成功完成，但裝置未連線至 VPN。**</span><span class="sxs-lookup"><span data-stu-id="7aacb-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="7aacb-112">成功狀態表示 Intune 已按照設定成功部署設定檔。</span><span class="sxs-lookup"><span data-stu-id="7aacb-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="7aacb-113">不過，這些設定可能不符合您的網路和/或驗證需求。</span><span class="sxs-lookup"><span data-stu-id="7aacb-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="7aacb-114">如需有關所嘗試連線的詳細資訊，請檢閱基礎結構和驗證服務 (VPN 伺服器和 NPS/RADIUS 伺服器) 中的記錄。</span><span class="sxs-lookup"><span data-stu-id="7aacb-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="7aacb-115">您可能需要與您的網路基礎結構小組或第三方 VPN 廠商合作，來收集和檢閱記錄。</span><span class="sxs-lookup"><span data-stu-id="7aacb-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="7aacb-116">**當我設定 iOS 版自訂 VPN 時，無法使用個別應用程式的 VPN 功能。**</span><span class="sxs-lookup"><span data-stu-id="7aacb-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="7aacb-117">iOS 裝置 Intune 中的個別應用程式 VPN 目前可供特定的提供者和合作夥伴使用，這些人在設定個別應用程式 VPN 之前，必須同時符合憑證先決條件。</span><span class="sxs-lookup"><span data-stu-id="7aacb-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="7aacb-118">如需詳細資訊，請參閱[iOS/iPadOS 裝置在 Intune 中設定個別應用程式虛擬私人網路 (VPN)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)。</span><span class="sxs-lookup"><span data-stu-id="7aacb-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="7aacb-119">如需有關 Intune 中所有 VPN 連線類型的詳細資訊，請參閱[建立 VPN 設定檔以連接到 Intune 中的 VPN 伺服器](https://docs.microsoft.com/intune/vpn-settings-configure)。</span><span class="sxs-lookup"><span data-stu-id="7aacb-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="7aacb-120">\*\*當存取已設定的網域時，未觸發 iOS 的隨選 VPN \*\*</span><span class="sxs-lookup"><span data-stu-id="7aacb-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="7aacb-121">若要測試自動 VPN 設定，請設定下列值：</span><span class="sxs-lookup"><span data-stu-id="7aacb-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="7aacb-122">我想要執行下列操作： **評估每個連線嘗試**</span><span class="sxs-lookup"><span data-stu-id="7aacb-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="7aacb-123">選擇是否要連線：**如有需要，請連線**</span><span class="sxs-lookup"><span data-stu-id="7aacb-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="7aacb-124">當使用者存取下列網域時： \**目標\*\*\*網域名稱*</span><span class="sxs-lookup"><span data-stu-id="7aacb-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="7aacb-125">如果上述設定失敗，請新增下列元素：</span><span class="sxs-lookup"><span data-stu-id="7aacb-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="7aacb-126">無法連線此 URL 時，強制連線 VPN：**BADURL**</span><span class="sxs-lookup"><span data-stu-id="7aacb-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>