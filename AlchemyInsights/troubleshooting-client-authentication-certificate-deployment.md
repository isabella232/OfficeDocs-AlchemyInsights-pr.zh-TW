---
title: 疑難排解用戶端驗證憑證部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658977"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="229e9-102">疑難排解用戶端驗證憑證部署</span><span class="sxs-lookup"><span data-stu-id="229e9-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="229e9-103">Intune NDES/SCEP 和 PKCS/PFX 用戶端憑證設定檔通常會結合其他設定檔類型 (例如 Wi-Fi、VPN 和電子郵件) 使用，以允許使用者驗證公司資源。</span><span class="sxs-lookup"><span data-stu-id="229e9-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="229e9-104">當這些設定檔類型與用戶端憑證連結時，設定檔會依賴於該設定檔的成功部署。</span><span class="sxs-lookup"><span data-stu-id="229e9-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="229e9-105">初始基礎結構設定和用戶端憑證設定檔相關聯的設定通常需要疑難排解。</span><span class="sxs-lookup"><span data-stu-id="229e9-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="229e9-106">如需成功設定 NDES 連接器的逐步指南，以及找出與憑證部署相關問題的疑難排解指導方針，請參閱：</span><span class="sxs-lookup"><span data-stu-id="229e9-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="229e9-107">設定基礎結構以使用 Intune 支援 SCEP</span><span class="sxs-lookup"><span data-stu-id="229e9-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="229e9-108">針對 SCEP 憑證設定檔搭配 Microsoft Intune 進行疑難排解的概觀</span><span class="sxs-lookup"><span data-stu-id="229e9-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="229e9-109">使用參考的 PowerShell 指令碼來協助驗證您的設定。</span><span class="sxs-lookup"><span data-stu-id="229e9-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="229e9-110">如需詳細資訊，請參閱 [Intune 憑證連接器驗證指令碼](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)。</span><span class="sxs-lookup"><span data-stu-id="229e9-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="229e9-111">**其他常見問題**</span><span class="sxs-lookup"><span data-stu-id="229e9-111">**Other common issues**</span></span>

<span data-ttu-id="229e9-112">**嘗試在 NDES 連接器伺服器上安裝 Intune 憑證連接器時，收到訊息：「無法驗證憑證要求中的密碼。它可能已經被使用。請取得新的密碼，與此要求一起提交。」**</span><span class="sxs-lookup"><span data-stu-id="229e9-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="229e9-113">此訊息表示您必須以系統管理員身分執行憑證連接器安裝。</span><span class="sxs-lookup"><span data-stu-id="229e9-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="229e9-114">在某些環境中，Intune 憑證執行所在的伺服器必須使用 Proxy 伺服器來連線到 Intune，因此憑證連接器必須使用 Proxy。</span><span class="sxs-lookup"><span data-stu-id="229e9-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="229e9-115">在某些情況下，NDES 連接器會忽略設定的 Proxy 設定，而且在 LocalSystem 的安全性環境中執行時，可能需要設定 Proxy 設定。</span><span class="sxs-lookup"><span data-stu-id="229e9-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="229e9-116">解決方案是以 SYSTEM 身分執行 Internet Explorer，並在 IE 中設定 Proxy。</span><span class="sxs-lookup"><span data-stu-id="229e9-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="229e9-117">將 Intune 連接器服務重新啟動之後，NDES 連接器就會連線到 Intune。</span><span class="sxs-lookup"><span data-stu-id="229e9-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="229e9-118">**使用者裝置不再會從 NDES 接收 SCEP 憑證。**</span><span class="sxs-lookup"><span data-stu-id="229e9-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="229e9-119">核發給 NDES 伺服器並在 NDES 連接器安裝期間指定的用戶端驗證憑證，可能已過期或遺失。</span><span class="sxs-lookup"><span data-stu-id="229e9-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="229e9-120">若要解決下列問題：</span><span class="sxs-lookup"><span data-stu-id="229e9-120">To resolve:</span></span> 
 
1. <span data-ttu-id="229e9-121">解除安裝 NDES 連接器。</span><span class="sxs-lookup"><span data-stu-id="229e9-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="229e9-122">使用這些詳細資料來要求新的用戶端驗證或伺服器驗證憑證：</span><span class="sxs-lookup"><span data-stu-id="229e9-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="229e9-123">主體名稱：CN=外部 FQDN</span><span class="sxs-lookup"><span data-stu-id="229e9-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="229e9-124">主體別名 (兩者都是必要)：DNS=外部 FQDN，DNS=內部 FQDN</span><span class="sxs-lookup"><span data-stu-id="229e9-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="229e9-125">使用新的憑證重新安裝 NDES 連接器。</span><span class="sxs-lookup"><span data-stu-id="229e9-125">Reinstall the NDES connector with the new certificate.</span></span>